数据的修改和删除

## 任务

查看当前表数据：

`[[SELECT * FROM bank_card where b_c_id<10 ORDER BY b_c_id;]]{{RUN}}`

更新数据，根据`client`表的`c_id`列更新`bank_card`表中`c_id<10`的所有行，设置`b_type`的值为`借记卡`：

`[[UPDATE bank_card SET bank_card.b_type='借记卡' from client where bank_card.b_c_id = client.c_id and bank_card.b_c_id<10;]]{{RUN}}`

重新查询数据情况：

`[[SELECT * FROM bank_card ORDER BY b_c_id;]]{{RUN}}`

按`q`返回交互模式。
