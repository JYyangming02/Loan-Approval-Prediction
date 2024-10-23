# Loan Approval Prediction 貸款核准預測
- [English](#English)  
- [繁體中文](#繁體中文)

---
## English

## Project Overview
This project focuses on predicting loan approval status using a machine learning pipeline that includes both preprocessing and model stacking techniques. The dataset was sourced from the [Kaggle Loan Approval Prediction competition](https://www.kaggle.com/competitions/playground-series-s4e10/overview).

## Data Preprocessing
- **Categorical Variables**:
  - For nominal (unordered) categorical variables, **one-hot encoding** was applied.
  - For ordinal (ordered) categorical variables, **label encoding** was used.
  
- **Class Imbalance Handling**:
  - Since the dataset has imbalanced classes, we applied both **oversampling** and **undersampling** techniques to balance the data.

## Model Architecture
This project leverages a **stacked ensemble learning** approach:
- **First Layer**: 
  - We used three models: **CatBoost**, **XGBoost**, and **LightGBM** to generate predictions.
- **Second Layer (Meta-Model)**:
  - An **Artificial Neural Network (ANN)** was used to combine the outputs of the first layer models, capturing deep insights from the data.

## Results
- The final model achieved **89% accuracy** on the validation set, showcasing its effectiveness in predicting loan approval.

## Dataset
- The dataset used in this project is from the [Kaggle Loan Approval Prediction competition](https://www.kaggle.com/competitions/playground-series-s4e10/overview).

# 貸款核准預測

## 繁體中文

## 專案概述
本專案旨在利用機器學習管道來預測貸款核准狀態，包含資料前處理與模型堆疊技術。資料來源來自[Kaggle貸款核准預測競賽](https://www.kaggle.com/competitions/playground-series-s4e10/overview)。

## 資料前處理
- **類別變項**:
  - 對於不具順序尺度的類別變項，使用**one-hot編碼**進行處理。
  - 對於具有順序尺度的類別變項，採用**標籤編碼**來進行轉換。
  
- **類別不平衡處理**:
  - 由於資料集中類別分布不均，我們使用了**上採樣**和**下採樣**技術來平衡資料。

## 模型架構
本專案採用了**集成式學習**中的**堆疊模型**方法：
- **第一層**: 
  - 使用了三個模型：**CatBoost**、**XGBoost** 和 **LightGBM** 來生成預測結果。
- **第二層 (Meta 模型)**:
  - 採用了**人工神經網路 (ANN)**，用以結合第一層模型的輸出，進一步獲取數據的深層特徵。

## 結果
- 最終模型在驗證集上達到了**89%的正確率**，顯示了該模型在貸款核准預測中的有效性。

## 資料集
- 本專案使用的資料集來自[Kaggle貸款核准預測競賽](https://www.kaggle.com/competitions/playground-series-s4e10/overview)。
