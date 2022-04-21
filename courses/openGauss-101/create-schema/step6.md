数据库创建完成后，就可以进行数据导入。

## 任务

在SQL编辑框中输入如下语句，对fund表进行数据初始化：

```
[[
INSERT INTO fund(f_name,f_id,f_type,f_amount,risk_level,f_manager) VALUES 
('股票',1,'股票型',10000,'高',1),
('投资',2,'债券型',10000,'中',2),
('国债',3,'货币型',10000,'低',3),
('沪深300指数',4,'指数型',10000,'中',4);
]]{{PRINT}}
```

查询fund表的插入条目数：
`[[select count(*) from fund;]]{{RUN}}`