# INSSqlStr
## SQL Server使用存储过程导出sql

--查询全部数据
    EXEC dbo.BuildINSSqlStr @Query = 'dbo.account_User where 1=1'  
    参数说明:  
    1.dbo.account_User：表  
    2.where 1=1：表示查询全部数据  
  
--带条件查询（查询用户为‘郭’的信息）
  EXEC dbo.BuildINSSqlStr @Query = 'dbo.account_User where LoginName=''郭'''  
  参数说明:  
  1.dbo.account_User：表  
  2.LoginName=''郭''：查询登录为郭的数据  
