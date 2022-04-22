删除数据

## 任务 

查看当前表数据：

`[[SELECT * FROM fund;]]{{RUN}}`

删除表`fund`中，`f_id<3`的数据条目：

`[[DELETE FROM fund WHERE f_id<3;]]{{RUN}}`

查询删除结果：

`[[SELECT * FROM fund;]]{{RUN}}`