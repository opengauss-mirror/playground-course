Schema创建完成后，就可以在该Schema下创建相应的数据表格

## 任务 

向finances_product表添加约束为finances_product表的p_amount列添加大于等于0的约束：

`[[ALTER table finances_product ADD CONSTRAINT c_p_mount CHECK (p_amount >=0);]]{{RUN}}`

尝试插入数据测试尝试手工插入一条金额小于0的记录，因为不满足约束条件，因此本条命令执行会失败：

`[[INSERT INTO finances_product(p_name,p_id,p_description,p_amount,p_year) VALUES ('信贷资产',10,'一般指银行作为委托人将通过发行理财产品募集资金委托给信托公司，信托公司作为受托人成立信托计划，将信托资产购买理财产品发售银行或第三方信贷资产。',-10,6);]]{{RUN}}`

向fund表添加约束为fund表的f_amount列添加大于等于0的约束：

`[[ALTER table fund ADD CONSTRAINT c_f_mount CHECK (f_amount >=0);]]{{RUN}}`

向insurance表添加约束 为insurance表的i_amount列添加大于等于0的约束：

`[[ALTER table insurance ADD CONSTRAINT c_i_mount CHECK (i_amount >=0);]]{{RUN}}`

验证约束的创建结果：

`[[select conname,connamespace,contype from pg_constraint where conrelid in (select oid from pg_class where relname in ('fund','insurance'));]]{{RUN}}`