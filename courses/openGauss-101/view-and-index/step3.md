在关系数据库中，索引是一种单独的、物理的对数据库表中一列或多列的值进行排序的一种存储结构，它是某个表中一列或若干列值的集合和相应的指向表中物理标识这些值的数据页的逻辑指针清单。索引的作用相当于图书的目录，可以根据目录中的页码快速找到所需的内容。索引提供指向存储在表的指定列中的数据值的指针，然后根据您指定的排序顺序对这些指针排序。数据库使用索引以找到特定值，然后顺指针找到包含该值的行。这样可以使对应于表的SQL语句执行得更快，可快速访问数据库表中的特定信息。

## 任务

在普通表property上创建索引：

`[[CREATE INDEX idx_property ON property(pro_c_id DESC,pro_income,pro_purchase_time);]]{{RUN}}`

重建property表的idx_property索引：

```
DROP INDEX idx_property;
CREATE INDEX idx_property ON property(pro_c_id DESC,pro_income,pro_purchase_time);
{{PRINT}}
```

索引重命名索引idx_property为idx_property_temp：

`[[ALTER INDEX idx_property RENAME TO idx_property_temp;]]{{RUN}}`

删除索引idx_property_temp：

`[[DROP INDEX idx_property_temp;]]{{RUN}}`