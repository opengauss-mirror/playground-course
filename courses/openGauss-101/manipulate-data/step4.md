本小节的金融数据库实验将会带领读者学习到更深一层的查询操作，让学习者能够更深入的去了解openGauss数据库的复杂操作。

## 任务

单表查询查询银行卡信息表：

`[[SELECT b_number,b_type FROM bank_card;]]{{RUN}}`

按`q`返回交互模式。

条件查询查询资产信息中‘可用’的资产数据：

`[[select * from property where pro_status='可用';]]{{RUN}}`

按`q`返回交互模式。

聚合查询查询用户表中有多少个用户：

`[[SELECT count(*) FROM client;]]{{RUN}}`

查询银行卡信息表中，储蓄卡和信用卡的个数：

`[[SELECT b_type,COUNT(*) FROM bank_card GROUP BY b_type;]]{{RUN}}`

查询保险信息表中，保险金额的平均值：

`[[SELECT AVG(i_amount) FROM insurance;]]{{RUN}}`

查询保险信息表中保险金额的最大值和最小值所对应的险种和金额：

```
[[
select i_name,i_amount from insurance where i_amount in (select max(i_amount) from insurance)
union
select i_name,i_amount from insurance where i_amount in (select min(i_amount) from insurance);
]]
{{PRINT}}
```