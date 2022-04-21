连接查询

## 任务

半连接查询用户编号在银行卡表中出现的用户的编号，用户姓名和身份证：

`[[SELECT c_id,c_name,c_id_card FROM client WHERE EXISTS (SELECT * FROM bank_card WHERE client.c_id = bank_card.b_c_id);]]{{RUN}}`

反连接查询银行卡号不是‘622202130202000001*’（*表示未知）的用户的编号，姓名和身份证：

`[[SELECT c_id,c_name,c_id_card FROM client WHERE c_id NOT IN (SELECT b_c_id FROM bank_card WHERE b_number LIKE '622202130202000001_');]]{{RUN}}`

按`q`返回交互模式。

