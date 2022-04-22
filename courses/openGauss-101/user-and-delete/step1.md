*Note: 本章节学习内容依赖于前面章节的数据及操作，请先前往前面章节完成相关的操作再进行本章学习*


## 任务

使用gsql工具登录数据库：

`[[gsql -d postgres -p 5432 -r -h 127.0.0.1]]{{RUN}}`

输入密码：
`openGauss@1234`

连接finance数据库：

`[[\connect finance]]{{RUN}}`

输入密码：
`openGauss@1234`

将默认搜索路径设为finance：
`[[SET search_path TO finance;]]{{RUN}}`
