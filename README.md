# Data Analysis Projects
## 1. Health Insurance Cross Sell Prediction 
(Kaggle dataset URL: https://www.kaggle.com/anmolkumar/health-insurance-cross-sell-prediction)

训练数据包含381109笔客户资料，每笔客户资料包含12个字段，1个客户ID字段、10个输入字段及1个目标字段-Response是否响应(1代表感兴趣，0代表不感兴趣)。

字段|角色|测量类型|不同值个数
---|---:|--:|--:
ID |记录标识|无类型|381109
Gender |输入|分类型|2
Age |输入|数值型|66
Driving_License |输入|分类型|2
Region_Code |输入|分类型|53
Previously_Insured |输入|分类型|2
Vehicle_Age |输入|分类型|3
Vehicle_Damage |输入|分类型|2
Annual_Premium |输入|数值型|48838
Policy_Sales_Channel |输入|分类|155
Vintage |输入|数值型|290
Response |目标|分类型|2

•	Goal: Build a model to predict whether a health insurance customer (policyholders) would be interested in vehicle insurance, which is helpful for the company to accordingly plan its communication strategy to reach out to those customers and optimise its business model and revenue.

•	Work done: Performed EDA analysis, data visualization and preprocessing based on 380k training data with 12 features in demographics, vehicle, and policy aspects. Conducted data modeling using various ML algorithms and hyperparameter tuning to improve the evaluation metric ROC_AUC score from 0.68 to 0.85.

Health Insurance Cross Sell Prediction/Health Insurance Cross Sell Prediction.ipynb
