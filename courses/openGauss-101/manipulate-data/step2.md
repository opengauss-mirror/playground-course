当C银行有新的信息需要加入数据库时，系统需要在对应的数据表中手动插入一条新的数据。


## 任务

在金融数据库的客户信息表中添加一个客户的信息（c_id_card和c_phone非唯一）：

`[[INSERT INTO client(c_id,c_name,c_mail,c_id_card,c_phone,c_password) VALUES (31,'李丽','lili@huawei.com','340211199301010005','18815650005','gaussdb_005');]]{{RUN}}`

会产生错误。

说明：由于在表的创建过程中，实验定义了c_id_card和c_phone为唯一且非空（UNIQUE NOT NULL），所以当表中存在时，插入数据失败。

在金融数据库的客户信息表中添加一个客户的信息：

`[[INSERT INTO client(c_id,c_name,c_mail,c_id_card,c_phone,c_password) VALUES (31,'李丽','lili@huawei.com','340211199301010031','18815650031','gaussdb_031');]]{{RUN}}`

检查插入的结果：

`[[select * from client where c_id=31;]]{{RUN}}`

按`q`返回交互模式。