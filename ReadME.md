# 🔍 Anomaly Detection & Data Quality Check

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange)
![Algorithm](https://img.shields.io/badge/Algorithm-Isolation%20Forest-green)

## 📖 Overview
This project focuses on **Automated Data Quality Checks** by identifying anomalies in Insurance datasets. Using the **Isolation Forest** algorithm (an unsupervised learning technique), the system automatically flags data points that deviate significantly from the norm—potentially indicating **fraud**, **data entry errors**, or **edge cases**.

## 🚀 Key Features
* **Outlier Detection:** Uses Isolation Forest to isolate anomalies without needing labeled data.
* **Data Quality Assessment:** Automatically flags rows that require manual review.
* **Visualization:** Plots normal vs. anomalous data points to visualize the decision boundary.
* **Scalable Logic:** The approach can be applied to financial transactions, network logs, or sensor data.

## 🛠️ Tech Stack
* **Python:** Core programming language.
* **Scikit-Learn:** For the `IsolationForest` model implementation.
* **Pandas & NumPy:** For data manipulation and preprocessing.
* **Matplotlib/Seaborn:** For visualizing the "Normal" vs. "Anomaly" distribution.

## 📊 Methodology
1.  **Data Ingestion:** Loads `insurance.csv` containing features like BMI, Age, Charges, etc.
2.  **Preprocessing:** Encodes categorical variables and scales numerical features.
3.  **Model Training:** Trains the Isolation Forest model to learn the distribution of "normal" data.
4.  **Prediction:** Assigns an anomaly score to each record; records with scores below a threshold are flagged as anomalies (-1).
5.  **Analysis:** visualizes the outliers to understand *why* they were flagged (e.g., unusually high charges for a young age).


## 📜 License
This project is open-source and available under the MIT License.
