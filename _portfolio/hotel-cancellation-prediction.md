---
title: "Hotel Booking Cancellation Prediction"
collection: portfolio
excerpt: "Built a predictive model to identify hotel booking cancellations and provide data-driven recommendations to reduce revenue loss."
date: 2025-12-01
---

## Project Background
Hotel booking cancellations can lead to significant revenue loss and operational inefficiency.  
This project aims to predict whether a booking will be cancelled based on customer and booking-related features, enabling better revenue management decisions.

## Data & Problem
- The dataset includes booking information such as lead time, deposit type, customer type, room preferences, and booking channels  
- The task is formulated as a **binary classification problem**: cancellation vs. non-cancellation  

## What I Did
- Cleaned and preprocessed raw booking data  
- Conducted exploratory data analysis (EDA) to identify patterns related to cancellation behavior  
- Performed feature engineering to improve model performance  
- Built and evaluated multiple classification models  
- Interpreted results from a **business perspective**, focusing on practical implications  

## Key Insights
- Lead time is one of the strongest predictors of cancellation  
- Bookings without deposits have significantly higher cancellation rates  
- Customer type and booking channels also show clear behavioral differences  
- The model can support overbooking and pricing strategy decisions  

## Tools & Skills
- Python (pandas, scikit-learn, matplotlib)  
- Classification models  
- Business analysis & data storytelling  

## Visual Preview
- Analysis Overview
![Hotel Cancellation Analysis Overview](/images/pipeline.png)
- Feature Importance
![Hotel Cancellation Analysis Feature](/images/Feature_Importance.png)
- Model Performance
![Hotel Cancellation Analysis Evaluation](/images/Model_performance.png)

## Full Report
📄 [Download the full project report (PDF)](/files/Hotel_reserve_cancellation_prediction_report.pdf)

---

## 中文项目摘要

本项目以酒店历史预订数据为基础，构建预测模型来判断订单是否会被取消，  
旨在帮助酒店提前识别高风险订单，从而减少因取消带来的收入损失。

### 问题定义
- 基于客户特征、预订信息及历史行为  
- 将问题建模为 **是否取消订单的二分类问题**

### 分析与建模过程
- 对原始数据进行清洗与预处理  
- 通过探索性数据分析（EDA）识别影响取消率的关键因素  
- 进行特征工程并构建多种分类模型进行对比  
- 从业务角度解读模型结果，而不仅关注模型指标本身  

### 核心结论
- 提前预订时间（Lead Time）对取消概率影响显著  
- 无押金订单的取消风险明显更高  
- 不同客户类型和预订渠道存在显著行为差异  

### 业务价值
- 可用于提前识别高风险订单  
- 为 overbooking 策略和收益管理提供数据支持  
- 辅助酒店制定更精细化的定价与客户管理策略  

📎 如需查看英文完整分析报告，可下载上方 PDF 文件。
