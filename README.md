# Higgs Boson Signal Classifier 

This project is a binary classifier built using CERN’s public Higgs Boson dataset.  

It aims to distinguish between **signal** events (potentially indicating the presence of a Higgs boson) and **background** events, based on high-level physics-derived features.

---

## Project Objective

The goal is to design a machine learning pipeline that effectively classifies events from particle collisions. This challenge was originally proposed by CERN as part of the Kaggle Higgs Boson competition.

---
## Dataset Description
The dataset consists of 250,000 events with 30 numerical features.  

It was released as part of the 2014 Kaggle Higgs Boson Challenge by CERN.

---
## Modeling Approach
A Gradient Boosting Classifier was selected due to its strong performance in tabular data with moderate imbalance and complex feature interactions.

---
## Model Performance

Despite the slight class imbalance in the dataset, the trained Gradient Boosting Classifier achieved a high classification performance.  

This indicates the model’s robustness and its ability to generalize well across both signal and background events.

---
## Techniques Used

- Exploratory Data Analysis
- Feature Scaling and Preprocessing
- Model Training with **Gradient Boosting Classifier**
- Hyperparameter Tuning using **GridSearchCV**
- Evaluation using:
  - **Accuracy Score**  
  - **ROC Curve & AUC Score**
  - **Confusion Matrix**

---

## Final Results

- **Accuracy:** 84.1%  
- **AUC Score:** ~0.91  
- Model exported using `joblib` and saved in `/models` directory

---

## Tech Stack

- Python
- Jupyter Notebook
- pandas, numpy
- matplotlib, seaborn
- scikit-learn

---

## Project Structure

```
higgs-boson-classifier/
├── data/                       
├── models/                     
│   └── higgs_classifier.joblib
├── classifier.ipynb           
├── requirements.txt           
└── README.md                  
```

---

## Dataset Source

- [Kaggle – Higgs Boson Challenge](https://www.kaggle.com/c/higgs-boson/data)
- Originally provided by CERN and ATLAS collaboration

---

## Future Work

- Converting this model into **FPGA-compatible code** using `hls4ml`  
- Evaluating latency and inference speed on edge devices  
- Potential integration into real-time classification tasks in particle detectors

---

## Author

**Ahmet Can Çömez**  
Computer Engineering Student  

