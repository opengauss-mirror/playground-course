子查询

## 任务

通过子查询，查询保险产品中保险金额大于平均值的保险名称和适用人群：

`[[SELECT i1.i_name,i1.i_amount,i1.i_person FROM insurance i1 WHERE i_amount > (SELECT avg(i_amount) FROM insurance i2);]]{{RUN}}`

`ORDER BY`和`GROUP BYORDER BY`子句按照保额降序查询保险编号大于`2`的保险名称，保额和适用人群：

`[[SELECT i_name,i_amount,i_person FROM insurance WHERE i_id>2 ORDER BY i_amount DESC;]]{{RUN}}`

`GROUP BY`子句 查询各理财产品信息总数，按照`p_year`分组：

`[[SELECT p_year,count(p_id) FROM finances_product GROUP BY p_year;]]{{RUN}}`

`HAVING`和`WITH ASHAVING`子句查询保险金额统计数量等于`2`的适用人群数：

`[[SELECT i_person,count(i_amount) FROM insurance GROUP BY i_person HAVING count(i_amount)=2;]]{{RUN}}`

备注：`HAVING`子句依附于`GROUP BY`子句而存在。

`WITH AS`子句使用`WITH AS`查询基金信息表：

`[[WITH temp AS (SELECT f_name,ln(f_amount) FROM fund ORDER BY f_manager DESC) SELECT * FROM temp;]]{{RUN}}`

备注：该语句为定义一个SQL片段，该SQL片段会被整个SQL语句用到。可以使SQL语句的可读性更高。存储SQL片段的表与基本表不同，是一个虚表。数据库不存放对应的定义和数据，这些数据仍存放在原来的基本表中。若基本表中的数据发生变化，从存储SQL片段的表中查询出的数据也随之改变。
