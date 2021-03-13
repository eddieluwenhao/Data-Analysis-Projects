# Data Analysis Projects
## 1. Health Insurance Cross Sell Prediction 
(Kaggle dataset URL: https://www.kaggle.com/anmolkumar/health-insurance-cross-sell-prediction)

为了预测客户是否对车辆保险感兴趣，获得有关人口统计数据(性别、年龄、地区编码类型)、车辆(车辆年龄、损坏情况)、保单(保费、采购渠道)等信息。

数据划分为训练集和测试集，训练数据包含381109笔客户资料，每笔客户资料包含12个字段，1个客户ID字段、10个输入字段及1个目标字段-Response是否响应(1代表感兴趣，0代表不感兴趣)。测试数据包含127037笔客户资料；字段个数与训练数据相同，目标字段没有值。字段的定义可参考下文。

字段|字段翻译|角色|测量类型|不同值个数
---|:--:|---:|--:|--:
ID |客户ID|记录标识|无类型|381109
Gender |性别|输入|分类型|2
Age |年龄|输入|数值型|66
Driving_License |是否有驾照|输入|分类型|2
Region_Code |用户所在区域的编码|输入|分类型|53
Previously_Insured |之前是否投保|输入|分类型|2
Vehicle_Age |车龄|输入|分类型|3
Vehicle_Damage |车辆损坏情况|输入|分类型|2
Annual_Premium |年度保费（卢比）|输入|数值型|48838
Policy_Sales_Channel |销售渠道|输入|分类|155
Vintage |往来时长（天）|输入|数值型|290
Response |是否响应|目标|分类型|2
