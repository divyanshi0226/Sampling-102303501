# Sampling Assignment – Credit Card Fraud Detection

## Objective
The objective of this assignment is to study the importance of sampling techniques while working with imbalanced datasets and to analyze how different sampling strategies affect the performance of various machine learning models.

---

## Dataset
The dataset used is the **Credit Card Fraud Detection Dataset**, which is highly imbalanced.
- Class `0`: Legitimate transactions  
- Class `1`: Fraudulent transactions  

The dataset was first converted into a **balanced dataset** using random undersampling.

---

## Sampling Techniques Used
The following sampling techniques were used as specified in the assignment:

1. Simple Random Sampling  
2. Systematic Sampling  
3. Stratified Sampling  
4. Cluster Sampling  
5. Bootstrap Sampling  

Cross-Validation was additionally used to evaluate model stability.

---

## Machine Learning Models Used
Five different machine learning models were trained on each sampling technique:

- Logistic Regression  
- Decision Tree  
- Random Forest  
- Support Vector Machine (SVM)  
- K-Nearest Neighbors (KNN)  

---

## Experimental Results

| Model / Sampling | Simple Random | Systematic | Stratified | Cluster | Bootstrap |
|------------------|--------------|------------|------------|---------|-----------|
| Logistic Regression | 33.33 | 0.00 | 16.67 | 50.00 | 100.00 |
| Decision Tree | 66.67 | 0.00 | 66.67 | 0.00 | 100.00 |
| Random Forest | 66.67 | 33.33 | 33.33 | 100.00 | 83.33 |
| SVM | 50.00 | 33.33 | 16.67 | 50.00 | 100.00 |
| KNN | 50.00 | 33.33 | 16.67 | 50.00 | 100.00 |

*(Values represent accuracy in percentage)*

---

## Analysis and Discussion
- Bootstrap Sampling performed the best overall, providing high accuracy for most models.
- Cluster Sampling worked exceptionally well with Random Forest but was unstable for simpler models.
- Systematic Sampling showed comparatively lower performance due to loss of class diversity in smaller samples.
- Ensemble models such as Random Forest were more robust to sampling variations compared to linear models.

---

## Conclusion
This study demonstrates that the choice of sampling technique plays a crucial role in model performance when dealing with imbalanced datasets. Bootstrap and Simple Random Sampling showed better generalization, while Stratified Sampling ensured balanced class representation.

---

## How to Run the Code
1. Upload `Creditcard_data.csv` to Google Colab.
2. Open `sampling_assignment.ipynb`.
3. Run all cells sequentially.
4. The final accuracy comparison table will be generated automatically.

---

## Author
Divyanshi
