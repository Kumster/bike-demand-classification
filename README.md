# 🚲 Capital Bikeshare Demand Classification

This project is part of my coursework in Machine Learning (DNSC6315) at George Washington University. The objective was to **predict whether the number of bike pickups (PU_ct) would exceed drop-offs (DO_ct)** using weather conditions and other features.

## 📌 Problem Statement

> Allocate more bikes if `PU_ct > DO_ct` and fewer if `PU_ct < DO_ct`.

We transform this into a binary classification task and compare multiple machine learning models to predict whether **"PU_High"** or **"DO_High"**.

## 📁 Dataset

- `202403-capitalbikeshare-tripdata.csv`: Real-world bike trip data.
- `DC_weather_2024.csv`: Hourly weather observations used to enhance features (e.g., temp, windspeed, icon).

## ⚙️ Features Used

- Temperature, windspeed, precipitation
- UV index
- Weather icon (one-hot encoded)

## 🧠 Models Compared

1. **Support Vector Classifier (Linear Kernel)**
2. **Decision Tree (max_depth=3, entropy)**
3. **K-Nearest Neighbors (K=10)**

## 📊 Evaluation Metrics

- Accuracy
- Area Under Curve (AUC)
- Confusion Matrix
- True Positive Rate (TPR) / False Positive Rate (FPR)

## 🏁 Final Results

| Model         | AUC (5-fold CV) | Test AUC |
|---------------|------------------|----------|
| SVC (Linear)  | 27.67%           | ✅ **38.75%** |
| Decision Tree | 36.58%           | --       |
| KNN (k=10)     | 50.17%           | --       |

✅ **SVC was selected** as the final model based on out-of-sample AUC.

## 📈 Visualization

![Tree](images/tree_visual.png)
![Confusion Matrix](images/confusion_matrix.png)

## 📚 Concepts Demonstrated

- Supervised learning (classification)
- Feature engineering
- Train-test split
- One-hot encoding
- Model evaluation: Accuracy, AUC, CV
- Model selection

## 🔧 Tools Used

- Python, Jupyter Notebook
- scikit-learn
- pandas, matplotlib, seaborn

---

👨‍💻 **Author**: Kumar Tare  
📫 [LinkedIn](https://linkedin.com/in/kumar-tare) | [Portfolio](https://yourdomain.com)
