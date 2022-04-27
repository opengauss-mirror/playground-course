<font color=darkred>*注意: 本章节学习内容依赖于前面章节的数据及操作，请先前往前面章节完成相关的操作再进行本章学习*</font>


## 任务

使用gsql工具登录`finance`数据库：

`[[gsql -d finance -p 5432 -r -h 127.0.0.1]]{{RUN}}`

输入密码：
`openGauss@1234`

将默认搜索路径设为`finance`：
`[[SET search_path TO finance;]]{{RUN}}`
