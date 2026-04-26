---
title: "酒店预订取消风险预测与经营优化分析"
collection: portfolio
excerpt: "本项目围绕酒店行业高频痛点——订单取消率高、库存损耗大、收益不稳定——展开，通过机器学习预测高风险取消订单，帮助酒店提前采取运营动作。最终在多模型比较后，选择 T=90 Logistic Regression（提前90天预测） 作为最优方案。"
author: academicpages
author_profile: true
date: 2025-12-01
header:
  teaser: /images/projects/hotel-teaser.jpg
---

## 业务背景
为解决酒店行业高频痛点——订单取消率高导致收益不稳定，本项目以酒店历史预订数据为基础，构建预测模型来判断订单是否会被取消，  
旨在帮助酒店提前识别高风险订单，从而减少因取消带来的收入损失。

## 方法
- 探索性分析 
- 特征工程
- Logistic Regression  
- Random Forest
![Hotel Cancellation Analysis Overview](/images/pipeline.png)
## 核心业务结论
**提前90天预测，比临近入住预测更有价值**

模型结果显示，提前90天预测的 F1-score 高于30天预测模型，且酒店拥有更长调整窗口。早预测可以1.提前释放潜在空房库存；2.更早启动二次销售 / 动态调价；3.提前安排人力与房态资源。

![Hotel Cancellation Analysis Feature](/images/hotel_table1.png)
![Hotel Cancellation Analysis Evaluation](/images/Model_performance.png)

**建议**
  
--建立取消风险预警系统，每日自动输出1.高风险订单名单；2.预计释放房间数3.高风险入住日期；用于收益管理团队决策。

--动态管理库存，若某日期高取消风险，应1.提前开放更多房量；2.调高公开售价减少超卖风险

**酒店取消行为并非随机，存在稳定模式**

  模型识别出10个关键变量，包括：

预订提前天数（lead time），历史取消次数，房价 ADR，修改订单次数，是否不可退款，特殊需求数量，停车位需求，周末入住天数等。

酒店可基于客户行为画像进行精细化运营，而不是被动等取消发生。

![Hotel Cancellation Analysis Feature](/images/Feature_Importance.png)
  
**客户的预订行为、价格偏好与取消政策之间存在明确规律**

通过热力图分析可见：

1.	提前预订客户更倾向选择不可退款方案，说明这类客户计划性更强且价格敏感，酒店可推出 Early Bird 预付产品，提前锁定收入并降低取消风险。
2.	拥有较多特殊需求的客户更偏好可退款订单，反映其更重视灵活性与入住体验，因此应提供弹性退改政策及增值服务，而非单纯低价策略。
3.	周末入住与工作日入住具有明显联动，中长住客户是稳定收益来源，可通过连住套餐、会员权益等方式提升整体房晚收入。
4.	高房价订单则更多来自散客客户，建议强化官网直销、OTA精准投放及高端房型营销，提升高利润客群占比。

整体而言，各变量之间相关性普遍较低，说明取消行为并非由单一因素决定，而是由预订时间、价格、客户需求及历史行为共同驱动。因此，酒店应从统一定价与统一退改政策，升级为基于客户分层的精细化收益管理模式。

![Hotel Cancellation Analysis Feature](/images/hotel_heatmap.png)

**建议：**

应进行客户分群运营：

**- 高取消用户：** 订金约束 + 提前确认

**- 稳定客户：** 会员优惠 + 快速入住通道

**- 高消费客户：** 增值服务升级

## 工具
- Python (pandas, scikit-learn, matplotlib)  
- 分类模型  

## 完整报告
📄 [Download the full project report (PDF)](/files/Hotel_reserve_cancellation_prediction_report.pdf)

📎 如需查看**英文**完整分析报告，可下载上方 PDF 文件。
