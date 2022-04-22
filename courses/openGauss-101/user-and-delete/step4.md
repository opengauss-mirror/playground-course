假设C银行的某新员工想要在自己的用户下去访问sys用户下的金融数据库，则该员工需要向sys申请添加相关权限


## 任务

创建用户dbuser，并赋予创建数据库的权限，创建用户“dbuser”，密码为“Gauss#3demo”：

`[[CREATE USER dbuser with createdb IDENTIFIED BY 'Gauss#3demo';]]{{RUN}}`

授权用户给用户dbuser授予finance数据库下bank_card表的查询和插入权限，并将SCHEMA的权限也授予dbuser用户：

`[[GRANT SELECT,INSERT ON finance.bank_card TO dbuser;]]{{RUN}}`

`[[GRANT ALL ON SCHEMA finance to dbuser;]]{{RUN}}`

退出数据库：

`[[\q]]{{RUN}}`

使用新用户连接finance数据库使用操作系统omm用户在新的窗口登录并执行以下命令，并在输入对应的密码：`Gauss#3demo`

`[[gsql -d finance -U dbuser -p 5432 -r -h 127.0.0.1]]{{RUN}}`

查询bank_card表数据 查询finance数据库的表bank_card中，b_c_id<10的数据条目：

`[[select * from finance. bank_card where b_c_id<10;]]{{RUN}}`

退出数据库：

`[[\q]]{{RUN}}`


