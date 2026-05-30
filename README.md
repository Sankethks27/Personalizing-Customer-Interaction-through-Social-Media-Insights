# ✈️ AeroReach Insights: Personalizing Customer Interaction through Social Media Insights

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=python&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=for-the-badge&logo=python&logoColor=white)

## 📌 Project Overview

AeroReach Insights is an aviation analytics company focused on helping airlines create personalized digital marketing campaigns through data-driven decision-making. This project leverages customer demographic information, social media engagement metrics, travel behavior, and device preferences to identify high-potential customers and optimize marketing strategies.

Using machine learning and customer segmentation techniques, the project enables airlines to deliver personalized travel offers, improve customer engagement, increase ticket purchases, and maximize marketing ROI.

---

## 🎯 Business Problem

Airlines often struggle to personalize customer interactions despite having access to valuable customer information from social media and digital platforms. Generic advertisements result in lower engagement and wasted marketing budgets.

The challenge is to:

* Identify customers most likely to purchase travel products.
* Segment travelers based on demographic and behavioral characteristics.
* Deliver personalized offers tailored to customer interests and device preferences.
* Improve digital advertising efficiency and conversion rates.

---

## 🚀 Project Objectives

### 1. Customer Segmentation

Group customers into meaningful segments based on travel behavior, engagement patterns, and demographic characteristics.

### 2. Marketing ROI Prediction

Predict the likelihood of a customer purchasing a travel product using machine learning models.

### 3. Device-Specific Ad Targeting

Develop separate predictive models for laptop and mobile users to optimize advertising effectiveness.

### 4. Personalized Marketing

Enable airlines to create targeted campaigns that improve engagement and ticket sales.

---

## 🏢 About AeroReach Insights

AeroReach Insights is a forward-thinking aviation technology firm dedicated to transforming airline marketing through advanced analytics, machine learning, and customer behavior insights.

The company helps airlines:

* Understand traveler preferences
* Optimize digital marketing campaigns
* Target high-value customers
* Increase conversion rates
* Improve customer loyalty
* Maximize marketing ROI

---

## 📊 Dataset Information

### Dataset Size

* **Rows:** 11,760
* **Columns:** 17

### Target Variable

* **Taken_product**

  * Yes = Customer purchased the product
  * No = Customer did not purchase the product

### Key Features

| Feature                                      | Description                       |
| -------------------------------------------- | --------------------------------- |
| UserID                                       | Unique customer identifier        |
| Yearly_avg_view_on_travel_page               | Average yearly travel page views  |
| preferred_device                             | Device used for login             |
| total_likes_on_outstation_checkin_given      | Likes given on travel check-ins   |
| yearly_avg_Outstation_checkins               | Average annual travel check-ins   |
| member_in_family                             | Family size                       |
| preferred_location_type                      | Preferred travel destination type |
| Yearly_avg_comment_on_travel_page            | Travel page engagement            |
| total_likes_on_outofstation_checkin_received | Social engagement received        |
| week_since_last_outstation_checkin           | Recent travel activity            |
| following_company_page                       | Brand following status            |
| montly_avg_comment_on_company_page           | Monthly company page interactions |
| working_flag                                 | Employment status                 |
| travelling_network_rating                    | Travel network influence score    |
| Adult_flag                                   | Age category                      |
| Daily_Avg_mins_spend_on_traveling_page       | Daily engagement duration         |

---

## 🔍 Exploratory Data Analysis (EDA)

### Key Findings

### Device Preference

* 90.58% of users access the platform via mobile devices.
* Indicates a strong need for mobile-first marketing strategies.

### Travel Preferences

Most preferred travel categories:

* Beach Destinations
* Financial Locations
* Historical Sites

### Customer Engagement

* Strong correlation between social interactions and platform engagement.
* Users receiving more likes on travel check-ins spend more time on the platform.

### Company Page Engagement

* Approximately 72% of users do not follow the company page.
* Significant opportunity to increase brand engagement.

### Demographics

* Majority of users are non-working individuals.
* Marketing campaigns can be tailored to this segment.

---

## 🧹 Data Cleaning & Preprocessing

The following preprocessing steps were performed:

### Missing Value Treatment

* Numerical Features → Median Imputation
* Categorical Features → Mode Imputation

### Data Quality Fixes

* Standardized device categories
* Corrected inconsistent labels
* Converted data types
* Removed invalid entries

### Outlier Treatment

* Identified using IQR and Boxplots
* Capped using 5th and 95th percentile thresholds

### Feature Engineering

* Removed `UserID`
* Added `customer_segment` using K-Means Clustering

### Encoding

* Label Encoding applied to categorical variables

---

## 🤖 Machine Learning Models

### 1️⃣ K-Means Clustering

**Purpose:** Customer Segmentation

Used to group customers based on:

* Travel behavior
* Travel page engagement
* Check-in activity
* Social interaction

**Business Value**

* Personalized campaigns
* Better customer understanding
* Improved offer targeting

---

### 2️⃣ Random Forest Classifier

**Purpose:** Marketing ROI Prediction

Predicts whether a customer is likely to purchase a travel product.

#### Advantages

* Handles high-dimensional data
* Reduces overfitting
* Provides feature importance insights

---

### 3️⃣ XGBoost Classifier

**Purpose:** Device-Specific Ad Targeting

Separate models were built for:

* Laptop Users
* Mobile Users

#### Benefits

* Higher prediction accuracy
* Faster execution
* Better handling of complex relationships

---

## 📈 Model Evaluation

Models were evaluated using:

### Classification Metrics

* Accuracy
* Precision
* Recall
* F1-Score
* Classification Report

### Validation Approach

* Train-Test Split
* Performance Comparison
* Device-specific evaluation

---

## 💡 Business Insights

### Customer Segmentation

Distinct customer groups were successfully identified based on travel behavior and engagement patterns.

### Marketing Optimization

The predictive model enables airlines to focus marketing budgets on customers with a higher probability of conversion.

### Mobile-First Strategy

Since over 90% of users access the platform via mobile devices, prioritizing mobile experiences can significantly improve engagement.

### Social Influence Matters

Travel-related social interactions strongly impact platform engagement and customer behavior.

### Personalized Campaigns

Segment-based recommendations can increase:

* Ticket sales
* Customer engagement
* Brand loyalty
* Marketing ROI

---

## 🛠️ Technology Stack

### Programming Language

* Python

### Libraries

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Plotly
* Scikit-Learn
* XGBoost

### Machine Learning

* K-Means Clustering
* Random Forest
* XGBoost

### Data Analysis

* Exploratory Data Analysis (EDA)
* Feature Engineering
* Statistical Analysis

---

## 📂 Project Structure

```text
AeroReach-Insights/
│
├── data/
│   ├── AeroReach Insights.csv
│
├── notebooks/
│   ├── EDA.ipynb
│   ├── Data_Preprocessing.ipynb
│   ├── Model_Building.ipynb
│
├── reports/
│   ├── Final_Report.pdf
│
├── images/
│   ├── visualizations
│
├── README.md
│
└── requirements.txt
```

### Execute Workflow

1. Data Cleaning
2. Exploratory Data Analysis
3. Customer Segmentation
4. Model Training
5. Evaluation & Insights

---

## 📌 Recommendations

* Prioritize mobile marketing strategies.
* Increase company-page engagement through personalized content.
* Use customer segmentation for targeted promotions.
* Implement hyperparameter tuning for improved performance.
* Integrate real-time social media signals for dynamic recommendations.

---

## 📚 Key Learnings

* Social media engagement is a strong predictor of travel behavior.
* Device-specific targeting improves campaign effectiveness.
* Customer segmentation enables personalized marketing at scale.
* Data-driven marketing significantly improves resource allocation.

---

## 🤝🏿 **Contributing**

**Project:** AeroReach Insights – Personalizing Customer Interaction through Social Media Insights

Developed as part of a Machine Learning and Business Analytics project focused on customer segmentation, predictive modeling, and digital marketing optimization. While this is primarily a showcase of my work, I welcome discussions, feedback, and collaborations on data science projects.

## 📧 **Contact**

**Sanketh Ks**  
- GitHub: [@Sankethks27](https://github.com/Sankethks27)
- LinkedIn: [Sanketh Ks](https://www.linkedin.com/in/sanketh-ks-181962273/)
- Email: sankethks27@gmail.com

---

⭐ **If you find this portfolio helpful or inspiring, please give it a star!** ⭐

---
