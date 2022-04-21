删除Schema


## 任务

使用gsql工具登录数据库：

`[[gsql -d finance -p 5432 -r -h 127.0.0.1]]{{RUN}}`

输入密码：
`openGauss@1234`

使用“\dn”查看数据库下的schema：

`[[\dn]]{{RUN}}`

设置默认查询路径设置默认查询路径search_path 为finance：

`[[set search_path to finance;]]{{RUN}}`

使用“\dt”命令可以看到在finance中的对象：

`[[\dt]]{{RUN}}`

使用DROP SCHEMA 命令尝试删除finance，会有报错，因为finance下存在对象：

`[[DROP SCHEMA finance;]]{{RUN}}`

使用DROP SCHEMA…..CASCADE进行级联删除，会将finance连同下的对象一起删除：

`[[DROP SCHEMA finance CASCADE;]]{{RUN}}`

使用“\dt”命令可以看到在finance和public中的对象，对象已删除：

`[[\dt]]{{RUN}}`

退出数据库：

`[[\q]]{{RUN}}`


