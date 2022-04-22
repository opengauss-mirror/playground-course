### Schema

`Schema`又称作模式。每个数据库包含一个或多个`Schema`。数据库中的每个`Schema`包含表和其他类型的对象。通过管理`Schema`，允许多个用户使用同一数据库而不相互干扰，可以将数据库对象组织成易于管理的逻辑组，同时便于将第三方应用添加到相应的`Schema`下而不引起冲突。


## 任务

使用gsql工具登录数据库：

`[[gsql -d postgres -p 5432 -r -h 127.0.0.1]]{{RUN}}`

输入密码：
`openGauss@1234`

创建数据库`finance`：

`[[CREATE DATABASE finance ENCODING 'UTF8' template = template0;]]{{RUN}}`

连接`finance`数据库：

`[[\connect finance]]{{RUN}}`

输入密码：
`openGauss@1234`

创建名为`finance`的`Schema`，并设置`finance`为当前的`Schema`。

`[[CREATE SCHEMA finance;]]{{RUN}}`

将默认搜索路径设为`finance`：
`[[SET search_path TO finance;]]{{RUN}}`
