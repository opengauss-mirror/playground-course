数据库创建完成后，就可以进行数据导入。

## 任务

在SQL编辑框中输入如下语句，对insurance表进行数据初始化:

```
[[
INSERT INTO insurance(i_name,i_id,i_amount,i_person,i_year,i_project) VALUES 
('健康保险',1,2000,'老人',30,'平安保险'),
('人寿保险',2,3000,'老人',30,'平安保险'),
('意外保险',3,5000,'所有人',30,'平安保险'),
('医疗保险',4,2000,'所有人',30,'平安保险'),
('财产损失保险',5,1500,'中年人',30,'平安保险');
]]{{PRINT}}
```

查询insurance表的插入条目数：
`[[select count(*) from insurance;]]{{RUN}}`