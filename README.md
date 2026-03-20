# Machine Learning Project: K-Nearest Neighbours vs Random Forest

This repository contains a machine learning project comparing **K-Nearest Neighbours (KNN)** and **Random Forest** classifiers on a glass classification dataset.

---

## Project Overview

- Implementation of KNN and Random Forest models using Python  
- Comparative analysis of model performance  
- Evaluation using classification metrics (accuracy, precision, recall, F1-score)  
- Analysis of differences in model behaviour across the dataset  

---

## Dataset

The dataset used in this project is a glass classification dataset, where the goal is to classify different types of glass based on their chemical properties.

**Source:**
https://www.kaggle.com/datasets/uciml/glass

---

## Methodology

- Data preprocessing and cleaning  
- Splitting the dataset into training and testing sets  
- Training classification models  
- Evaluating performance using standard classification metrics  

---

## Results

| Model            | Accuracy | Macro Precision | Macro Recall | Macro F1 |
|------------------|----------|-----------------|--------------|----------|
| KNN              | 0.79     | 0.74            | 0.70         | 0.70     |
| Random Forest    | 0.81     | 0.83            | 0.74         | 0.77     |

---

## Analysis

The results show that Random Forest outperforms K-Nearest Neighbours across most evaluation metrics, achieving higher overall accuracy (0.81 vs 0.79) and stronger macro-averaged precision, recall, and F1-score.

A key observation is that KNN struggled to correctly classify certain classes (e.g., class 3), where it failed to identify any instances. In contrast, Random Forest was able to detect these minority classes more effectively, although performance remained limited due to class imbalance.

This suggests that Random Forest is better suited for capturing more complex patterns in the dataset, while KNN is more sensitive to class distribution and distance-based limitations.

Overall, the results highlight the importance of model choice when dealing with imbalanced classification problems. This comparison demonstrates how ensemble methods can provide more robust performance than instance-based methods in complex classification tasks.

---

## Technologies Used

- Python  
- scikit-learn  
- Pandas  
- NumPy  

---

## Future Work

- Hyperparameter tuning for improved performance  
- Testing additional classification models  
- Applying cross-validation for more robust evaluation  

---

## Notes

This project was developed as part of coursework and independent study to explore model evaluation and comparison in machine learning.
