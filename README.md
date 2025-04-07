# 📊 Big Data Classification with PySpark

This project demonstrates a complete pipeline for handling, processing, and modeling a **large healthcare dataset** using **Apache Spark (PySpark)**. The goal is to predict ICU admission (risk) in patients using classification models, while addressing **missing values**, **class imbalance**, and **cluster-based learning**.

## 🚀 Project Overview

The project is part of a Big Data assignment and includes the following:

- Data cleaning & imputation of missing values
- Feature transformation and scaling
- Binary classification using Logistic Regression
- Class balancing using oversampling (SMOTE)
- Clustering using KMeans (with PCA visualization)
- Cluster-wise classifier training and evaluation
- Model performance comparison (Global vs. Clustered)

## 📂 Project Structure

```bash
📁 project-root/
├── Report.pdf                    # Sample report template
├── BigData.ipynb (converted)    # Original code in Colab format
├── README.md                     # This file
├── output_images/               # Screenshots of evaluation results


🔧 Technologies Used
Apache Spark (PySpark)

Pandas & Matplotlib (for cluster visualization)

Sklearn (for precision/recall/F1 metrics and SMOTE)

KMeans (via PySpark MLlib)

Logistic Regression

Google Colab / Jupyter

🧪 Model Performance
Global Model (Logistic Regression)
AUC: 0.771

Precision: 0.876

Recall: 0.751

F1-score: 0.792

After Balancing
AUC: 0.772

Precision: 0.720

Recall: 0.711

F1-score: 0.708

Cluster-Based Models
Cluster ID	AUC	Size
Cluster 0	0.668	72,100
Cluster 1	0.615	94,656
Cluster 2	0.654	33,275
📌 Key Insights
Imputation of missing values was done using mean (for AGE) and mode (for categorical features, including a two-step logic for PREGNANT).

Balancing the dataset using SMOTE improved recall but reduced precision.

The global model outperformed the cluster-specific models, though cluster-wise classification showed promise in specific segments (especially Cluster 0).

KMeans clustering with PCA helped visualize data separability and identify patterns in patient profiles.

📷 Sample Visuals
Elbow method for optimal K

PCA-based cluster visualization

ROC-AUC comparisons

Confusion matrices before and after balancing

📝 Conclusion
This project highlights the importance of:

Data preprocessing for large-scale healthcare data,

Evaluating the trade-off between global vs. segmented modeling,

The effectiveness of class balancing in improving minority class detection.

🙌 Acknowledgements
Special thanks to the [Big Data module] coursework for providing the dataset and assignment structure.


Let me know if you want to include a **demo GIF**, **Colab link**, or a **license section** too.
