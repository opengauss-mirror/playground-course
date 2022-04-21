Schema创建完成后，就可以在该Schema下创建相应的数据表格

## 任务 

在SQL编辑框中输入如下语句，创建客户信息表client：

```
[[
CREATE TABLE client
(
        c_id INT PRIMARY KEY,
        c_name VARCHAR(100) NOT NULL,
        c_mail CHAR(30) UNIQUE,
        c_id_card CHAR(20) UNIQUE NOT NULL,
        c_phone CHAR(20) UNIQUE NOT NULL,
        c_password CHAR(20) NOT NULL
);
]]{{PRINT}}
```

在SQL编辑框中输入如下语句，创建银行卡信息表bank_card：

```
[[
CREATE TABLE bank_card
(
        b_number CHAR(30) PRIMARY KEY,
        b_type CHAR(20),
        b_c_id INT NOT NULL
);
]]{{PRINT}}
```

在SQL编辑框中输入如下语句，创建理财产品信息finances_product：
```
[[
CREATE TABLE finances_product
(
        p_name VARCHAR(100) NOT NULL,
        p_id INT PRIMARY KEY,
        p_description VARCHAR(4000),
        p_amount INT,
        p_year INT
);
]]{{PRINT}}
```

创建保险信息表insurance

```
[[
CREATE TABLE insurance
(
        i_name VARCHAR(100) NOT NULL,
        i_id INT PRIMARY KEY,
        i_amount INT,
        i_person CHAR(20),
        i_year INT,
        i_project VARCHAR(200)
);
]]{{PRINT}}
```

在SQL编辑框中输入如下语句，创建保险信息表fund：
```
[[
CREATE TABLE fund
(
        f_name VARCHAR(100) NOT NULL,
        f_id INT PRIMARY KEY,
        f_type CHAR(20),
        f_amount INT,
        risk_level CHAR(20) NOT NULL,
        f_manager INT NOT NULL
);
]]{{PRINT}}
```

在SQL编辑框中输入如下语句，创建资产信息表property：
```
[[
CREATE TABLE property
(
        pro_id INT PRIMARY KEY,
pro_c_id INT NOT NULL,
        pro_pif_id INT NOT NULL,
        pro_type INT NOT NULL,
        pro_status CHAR(20),
        pro_quantity INT,
        pro_income INT,
        pro_purchase_time DATE
);
```
