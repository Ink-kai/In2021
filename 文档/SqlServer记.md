## mssql

### 字符串函数

+ substring(exp,start,length)	截断/分割/截取

  `select substring('ink-kai',5,6)`	// kai

+ stuff(exp,start,length,替换字符)  删除指定长度的字符，并在指定的起点处插入另一组字符。

+ for xml path(‘’) 聚合多行，转xml，一般都是结合stuff使用

  ```sql
  select ','+字段 from 表 for xml path('')
  ```

  

### 小记

+ 20210331

  #### distinct是将所有查询的字段进行对比去重，所有字段都完全相同才会去重

  #### distinct 必须放在查询字段开头进行查询

  #### group by 根据字段进行去重，字段相同就会去重

