数据库创建完成后，就可以进行数据导入。

## 任务

在SQL编辑框中输入如下语句，对`property`表进行数据初始化:

```
[[
INSERT INTO property(pro_id,pro_c_id,pro_pif_id,pro_type,pro_status,pro_quantity,pro_income,pro_purchase_time) VALUES 
(1,5,1,1,'可用',4,8000,'2018-07-01'),
(2,10,2,2,'可用',4,8000,'2018-07-01'),
(3,15,3,3,'可用',4,8000,'2018-07-01'),
(4,20,4,1,'冻结',4,8000,'2018-07-01');
]]{{RUN}}
```

查询`property`表的插入条目数：
`[[select count(*) from property;]]{{RUN}}`