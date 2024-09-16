# E-commerce Customer Segmentation

[![Python Version](https://img.shields.io/badge/python-3.12%2B-blue)](https://www.python.org/downloads/)

![AakashMehtaCustomerIsKingGIF](https://github.com/user-attachments/assets/056b73bc-b2d3-42f2-9a95-ae32a5a803d3)


## Table of Contents

- [E-commerce Customer Segmentation and Purchase Prediction](#e-commerce-customer-segmentation-and-purchase-prediction)
  - [Table of Contents](#table-of-contents)
  - [Abstract](#abstract)
  - [Introduction](#introduction)
  - [Methodology](#methodology)
    - [Data Preprocessing](#data-preprocessing)
    - [Exploratory Data Analysis](#exploratory-data-analysis)
    - [Feature Engineering](#feature-engineering)
    - [Customer Segmentation](#customer-segmentation)
    - [Purchase Prediction](#purchase-prediction)
  - [Results](#results)
  - [Discussion](#discussion)
  - [Installation](#installation)
  - [Usage](#usage)
  - [Contributing](#contributing)
  - [License](#license)
  - [Acknowledgments](#acknowledgments)
  - [References](#references)

## Abstract

This repository presents a comprehensive analysis of customer segmentation and purchase prediction in the e-commerce domain. Utilizing advanced machine learning techniques, we demonstrate the efficacy of K-means clustering for customer segmentation and evaluate multiple supervised learning algorithms for predicting future purchases. Our findings contribute to the growing body of literature on consumer behavior analysis in digital marketplaces.

## Introduction

In the rapidly evolving landscape of e-commerce, understanding customer behavior is paramount for business success. This study addresses two critical objectives:

1. Classification of customers into distinct segments based on purchase behavior and demographics.
2. Prediction of future purchases for new customers during their initial year, leveraging only first-purchase data.

These objectives align with the current research trends in customer relationship management (CRM) and predictive analytics in e-commerce (Kumar et al., 2020; Wang et al., 2019).

## Methodology

### Data Preprocessing

Our analysis begins with rigorous data preprocessing to ensure the integrity and reliability of our dataset. This process includes:

- Handling missing values, particularly in the `CustomerID` field
- Removal of duplicate entries
- Data type verification and conversion

### Exploratory Data Analysis

We conduct a thorough exploratory data analysis (EDA) to uncover underlying patterns and distributions within our dataset. This phase includes:

- Univariate analysis of categorical and continuous variables
- Visualization of key metrics using matplotlib and seaborn
- Identification and treatment of outliers

### Feature Engineering

To enhance the predictive power of our models, we employ various feature engineering techniques, including:

- Creation of derived features (e.g., average order value, purchase frequency)
- Encoding of categorical variables
- Normalization of numerical features

### Customer Segmentation

For customer segmentation, we implement the K-means clustering algorithm. The optimal number of clusters is determined through the elbow method and silhouette analysis (Kodinariya & Makwana, 2013).

### Purchase Prediction

We evaluate four machine learning models for purchase prediction:

1. Logistic Regression
2. Decision Tree
3. Random Forest
4. k-Nearest Neighbors
5. Support Vector Machine (SVC
6. Gradient Boosting Classifier
7. AdaBoost Classifier
8. Voting Classifier (RF + GB + kNN)

These models are chosen based on their proven efficacy in similar e-commerce contexts (Chen & Guestrin, 2016; Liaw & Wiener, 2002).

## Results

Our analysis yielded the following performance metrics for purchase prediction:

| Model                             | Train Accuracy (%) | Test Accuracy (%) |
| --------------------------------- | ------------------ | ----------------- |
| Support Vector Machine (SVC)      | 87.40              | 71.03             |
| Logistic Regression               | 91.27              | 75.46             |
| k-Nearest Neighbors               | 78.53              | 67.89             |
| Decision Tree                     | 84.63              | 71.38             |
| Random Forest                     | 90.30              | 74.99             |
| AdaBoost Classifier               | 53.88              | N/A               |
| Gradient Boosting Classifier      | 89.34              | 74.75             |
| Voting Classifier (RF + GB + kNN) | 91.00              | 75.58             |

## Discussion

The high training accuracy across models suggests potential overfitting, especially in the case of the Random Forest. Future work should focus on regularization techniques and cross-validation to improve generalization. k-Nearest Neighbors gives more stable results (judging by comparable Training & Testing accuracies)

## Installation

To set up the project environment:

```bash
git clone https://github.com/riziuzi/ecommerce-customer-segmentation.git
cd ecommerce-customer-segmentation
pip install -r requirements.txt
```

## Contributing

![PullrequestGIF](https://github.com/user-attachments/assets/9e27c9e0-640b-485a-b89d-1fc1ee9cbe00)

We welcome contributions to this project. Please follow these steps:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Acknowledgments

We extend our gratitude to the open-source community and the authors of the libraries used in this project.

---

created by **[riziuzi](https://github.com/riziuzi)**
