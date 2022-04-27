数据库创建完成后，就可以进行数据导入。

## 任务

在SQL编辑框中输入如下语句，对`bank_card`表进行数据初始化执行`insert`操作：

```
[[
INSERT INTO bank_card(b_number,b_type,b_c_id) VALUES 
('6222021302020000001','信用卡',1),
('6222021302020000002','信用卡',3),
('6222021302020000003','信用卡',5),
('6222021302020000004','信用卡',7),
('6222021302020000005','信用卡',9),
('6222021302020000006','信用卡',10),
('6222021302020000007','信用卡',12),
('6222021302020000008','信用卡',14),
('6222021302020000009','信用卡',16),
('6222021302020000010','信用卡',18),
('6222021302020000011','储蓄卡',19),
('6222021302020000012','储蓄卡',21),
('6222021302020000013','储蓄卡',7),
('6222021302020000014','储蓄卡',23),
('6222021302020000015','储蓄卡',24),
('6222021302020000016','储蓄卡',3),
('6222021302020000017','储蓄卡',26),
('6222021302020000018','储蓄卡',27),
('6222021302020000019','储蓄卡',12),
('6222021302020000020','储蓄卡',29);
]]{{RUN}}
```

查询`bank_card`表的插入条目数：
`[[select count(*) from bank_card;]]{{RUN}}`