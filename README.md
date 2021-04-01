# Data Analysis Projects
## 1. [Health Insurance Cross Sell Prediction](https://github.com/eddieluwenhao/Data-Analysis-Projects/blob/main/1.%20Health%20Insurance%20Cross%20Sell%20Prediction/Health%20Insurance%20Cross%20Sell%20Prediction.ipynb)
(Kaggle dataset URL: https://www.kaggle.com/anmolkumar/health-insurance-cross-sell-prediction)

### Overview:
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

### Goal: 
Build a model to predict whether a health insurance customer (policyholders) would be interested in vehicle insurance, which is helpful for the company to accordingly plan its communication strategy to reach out to those customers and optimise its business model and revenue.

### Work done: 
Performed EDA analysis, data visualization and preprocessing based on 380k training data with 12 features in demographics, vehicle, and policy aspects. Conducted data modeling using various ML algorithms and hyperparameter tuning to improve the evaluation metric ROC_AUC score from 0.68 to 0.85.



## 2. [Credit Risk Scorecard Modeling & Default Prediction](https://github.com/eddieluwenhao/Data-Analysis-Projects/blob/main/2.%20Credit%20Risk%20Scorecard%20Modeling%20%26%20Default%20Prediction/Credit%20Risk%20Scorecard%20Modeling%20%26%20Default%20Prediction.ipynb)
(Kaggle dataset URL: https://www.kaggle.com/c/GiveMeSomeCredit/data)

### Overview:
根据15万的样本数据，建立一套基于评分卡的风控模型，最终根据客户的各种属性和行为数据，利用信用评分模型，对客户的信用进行评分，从而决定是否给予授信，授信的额度和利率，减少在金融交易中存在的交易风险

字段|说明|类型
---|---|---
SeriousDlqin2yrs|90天以上逾期或更差|Y/N
Age|年龄|整数
RevolvingUtilizationOfUnsecuredLines|除房地产和汽车贷款等无分期付款债务外，信用卡和个人信用额度的总余额除以信贷限额|百分比
DebtRatio|债务比(每月偿还的债务，赡养费，生活费除以每月的总收入)|百分比
MonthlyIncome|每月收入|实数
NumberOfOpenCreditLinesAndLoans|公开贷款(如汽车贷款或抵押贷款)和信用额度(如信用卡)的数量|整数
NumberRealEstateLoansOrLines|抵押贷款和房地产贷款的额度(包括房屋净值信贷)|整数
NumberOfTime30-59DaysPastDueNotWorse|借款人逾期30-59天的次数，但在过去两年没有更糟|整数
NumberOfTime60- 89DaysPastDueNotWorse|借款人逾期60-89天的次数，但在过去 两年没有更糟|整数
NumberOfTimes90DaysLate|借款人逾期90天(或以上)的次数|整数
NumberOfDependents|除自己(配偶、子女等)以外的家庭受养人人数|整数

### Steps to develop the Scorecard Model:
* Step1：数据获取，包括获取存量客户及潜在客户的数据存量客户，已开展融资业务的客户，包括个人客户和机构客户; 潜在客户，将要开展业务的客户
* Step2：EDA，获取样本整体情况，进行直方图、箱形图可视化 
* Step3：数据预处理，包括数据清洗、缺失值处理、异常值处理
* Step4：变量筛选，使用IV值衡量自变量的预测能力，筛选IV值>0.1的特征字段
* Step5：模型开发，包括变量分段bin、变量的WOE(证据权重)变换和逻辑回归估算三个部分
* Step6：模型评估，评估模型的区分能力、预测能力、稳定性，并形成模型评估报告，得出模型是否可以使用的结论
* Step7：生成评分卡(信用评分)，根据逻辑回归的系数和WOE等确定信用评分的方法，将Logistic模型转换为标准评分的形式
* Step8：建立评分系统(布置上线)，根据生成的评分卡，建立自动信用评分系统

### Result:
迭代优化所建立的Scorecard，通过LR超参数调整，改变feature的IV值筛选，调整分箱bin等方式，对LR Model进行评估提高evaluation metric ROC_AUC score至0.82.

