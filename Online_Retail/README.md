# Customer Segmentation & Churn Prediction - Online Retail

## Overview
This project focuses on **Customer Segmentation** and **Churn Prediction** using the **Online Retail II** dataset. Customer segmentation helps businesses understand different groups of customers based on their behavior, while churn prediction identifies customers who are likely to leave, enabling businesses to take proactive measures.

In this project, we applied machine learning algorithms such as **K-Means** for customer segmentation and **K-Nearest Neighbors (KNN)** for churn prediction. The project involves data preprocessing, exploratory data analysis (EDA), and feature engineering.

## Project Structure
'''
Online_Retail/
|                  
│   ├── data/                        # Dataset for Online Retail
│   ├── notebook                     # Jupyter notebook for this project
│   └── README.md                    # Detailed README for Online Retail project
'''

## Dataset
The **Online Retail II** dataset contains all the transactions occurring for a UK-based non-store online retailer between **2009 and 2011**. The company primarily sells unique giftware. The dataset includes the following attributes:

- **Invoice**: Unique invoice number.
- **StockCode**: Product code.
- **Description**: Product description (with some missing values).
- **Quantity**: Number of products per transaction.
- **InvoiceDate**: Date and time of the transaction.
- **Price**: Price per unit of product.
- **Customer ID**: Unique customer identifier (with some missing values).
- **Country**: Country of the customer.

Source: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Online+Retail+II)

## Installation
To run this project, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/ShravyaDsouza/CustomerSegmentationAndChurnPrediction.git

2. Navigate to the Online_Retail project folder:
   
   ```bash
   cd CustomerSegmentationAndChurnPrediction/Online_Retail

3. Install the required dependencies:

   ```bash
   pip install -r requirements.txt

## Usage
1. Load the dataset into the data/ folder of the corresponding project.
2. Open and run the Jupyter notebook:
   ```bash
   jupyter notebook "CustomerSegmentation&ChurnPrediction.ipynb"

## Models and Techniques

### Customer Segmentation:

- **K-Means Clustering** is used to segment customers based on their purchase behavior (e.g., quantity, spending patterns).
- Instead of the **Inertia** metric, other evaluation techniques such as the **Silhouette Score** and the **Elbow Method** are used to assess clustering performance.
- The best **Silhouette Score** achieved was `0.93`, indicating well-defined clusters.

### Churn Prediction:

- **K-Nearest Neighbors (KNN)** is used to predict customer churn based on their transaction history.
- The model is evaluated using metrics like **accuracy score**, **confusion matrix**, and **classification report**.
- The model achieved an **accuracy score** of `0.9984`, demonstrating high performance in predicting churn.

## Evaluation Metrics

- **Silhouette Score**: The best silhouette score was `0.93`, which indicates well-separated and well-defined clusters.
- **Elbow Method**: Helped determine the optimal number of clusters based on the rate of reduction in WCSS (Within-Cluster Sum of Squares).
- **Confusion Matrix**: Shows true positives, false positives, true negatives, and false negatives for the KNN model.
- **Accuracy Score**: The KNN model achieved an accuracy of `0.9984` for churn prediction.

## Results

### Customer Segmentation:

- The optimal number of clusters was determined using the **Elbow Method** and **Silhouette Score**.
- The **Silhouette Score** of `0.93` indicates that the clusters are well-formed and distinct from each other.
- Customers were grouped into segments based on purchasing patterns, providing valuable insights for targeted marketing strategies.

### Churn Prediction:

- The **KNN model** achieved a high **accuracy** of `0.9984` in predicting customer churn, helping identify customers at risk of leaving.

## Contributing

Contributions are welcome! If you have suggestions for improving the project or want to add additional features, feel free to fork the repository and submit a pull request.

