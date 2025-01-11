# 🌟 Air Quality Prediction Project 🌍

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Enabled-brightgreen?logo=sklearn&logoColor=white)
![Dataset](https://img.shields.io/badge/Dataset-Air%20Quality%20UCI-yellow?logo=open-access&logoColor=white)
![License](https://img.shields.io/badge/License-GPLv3-orange?logo=gnu&logoColor=white)

## 📜 Project Overview

This project uses machine learning techniques to predict **carbon monoxide (CO) levels** based on air quality attributes. By analyzing data from gas sensor arrays, the project aims to improve air quality forecasting and help protect public health and the environment.

### 📚 Course Details
- **Course Title**: Artificial Intelligence  
- **Course Code**: CSE 422  
- **Section**: 14  
- **Group**: 07  
- **Date**: 6th January 2025  

### 👩‍💻 Team Members
- **Arnab Das** - 19301029
- **Meshkatul Arefin** - 24341079

## 📖 Table of Contents
1. [Introduction](#introduction)
2. [Dataset Description](#dataset-description)
3. [Data Preprocessing](#data-preprocessing)
4. [Machine Learning Models](#machine-learning-models)
5. [Results & Analysis](#results--analysis)
6. [Conclusion](#conclusion)
7. [References](#references)

---

## 📌 Introduction
Carbon monoxide is a dangerous pollutant, and its high levels can cause serious health issues. Forecasting CO levels helps protect the environment and public health. This project implements machine learning to predict CO levels using the **Air Quality UCI dataset**.

---

## 📊 Dataset Description

- **Source**: [Air Quality UCI Dataset](https://archive.ics.uci.edu/ml/datasets/Air+Quality)
- **Size**: 9,357 rows, 16 columns

### Key Features
- **CO_GT**: Carbon monoxide levels (mg/m³)
- **PT08_S1_CO**: Sensor data for CO
- **NMHC_GT**: Non-methanic hydrocarbon levels (microg/m³)
- **NO2_GT**: Nitrogen dioxide levels (microg/m³)
- **T**: Temperature (°C)
- **RH**: Relative humidity (%)

---

## 🔄 Data Preprocessing

### 1. Missing Value Treatment
- Replaced missing values (`-200`) with NaN.
- Column `NMHC_GT` was removed due to excessive missing values.
- Remaining NaN values were filled using column means.

### 2. Scaling
- Applied **MinMaxScaler** to normalize features to a range of [0, 1].

### 3. Train-Test Split
- Training data: 70%
- Testing data: 30%

---

## 🤖 Machine Learning Models

### 1. Decision Tree Classifier
- **Training Accuracy**: 1.0  
- **Testing Accuracy**: 1.0  
- Observed overfitting.

### 2. Random Forest Classifier
- **Training Accuracy**: 1.0  
- **Testing Accuracy**: 0.9968  
- Best performance, minimal overfitting.

### 3. K-Nearest Neighbors (KNN)
- **Training Accuracy**: 0.94  
- **Testing Accuracy**: 0.8857  
- Underperformed compared to tree-based models.

---

## 📈 Results & Analysis

- **Random Forest** was the most balanced model with high accuracy and minimal overfitting.
- **Decision Tree** performed perfectly but raised concerns of overfitting.
- **KNN** struggled to generalize and achieved lower scores.

### Performance Metrics (Testing)
| Model               | Precision | Recall |
|---------------------|-----------|--------|
| Decision Tree       | 1.0000    | 1.0000 |
| Random Forest       | 0.9968    | 0.9968 |
| K-Nearest Neighbor  | 0.8857    | 0.8857 |

---

## 🏁 Conclusion
Machine learning models like **Random Forest** and **Decision Tree** excel at air quality prediction. Random Forest is the recommended model due to its balance of accuracy and generalization. These insights can help authorities monitor and improve air quality.

---

## 🔗 References
- **U.S. Environmental Protection Agency (2022)**: [Carbon monoxide pollution in outdoor air](https://www.epa.gov/co-pollution)
- **Dataset**: [Air Quality UCI Dataset](https://archive.ics.uci.edu/ml/datasets/Air+Quality)

---

![BRAC University](https://img.shields.io/badge/BRAC-University-red?logo=brac&logoColor=white)
