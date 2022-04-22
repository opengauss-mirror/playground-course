创建完成的视图可以进行修改

## 任务 

修改视图内容修改视图，在原有查询的基础上，过滤出信用卡用户：

`[[CREATE OR REPLACE VIEW v_client as SELECT c_id,c_name,c_id_card FROM client WHERE EXISTS (SELECT * FROM bank_card WHERE client.c_id = bank_card.b_c_id and bank_card.b_type='信用卡');]]{{RUN}}`

使用视图进行查询：

`[[select * from v_client;]]{{RUN}}`

修改视图名称：

`[[ALTER VIEW v_client RENAME TO v_client_new;]]{{RUN}}`

将v_client视图删除，删除视图不会影响基表：

`[[DROP VIEW v_client_new;]]{{RUN}}`
