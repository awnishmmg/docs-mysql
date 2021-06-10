# docs-mysql
This is a Simple Blog for Mysql Documentation

# Different to perform soft delete.
1. use is_deleted and set default to 0 or 1
2. use deleted_at and set default to NULL
3. when you delete just update the time
4. Note : date('Y-m-d H:i:s') is Equivalent to Now() in mysql.
5. always make 6 fields at compulsory end created_at,updated_at,deleted_at,[taking current_timestamp() = timestamp/datetime] and created_at,updated_at,deleted_by
6. These 6 Fields are so powerful that it can hold any type of data you wanna keep.
7. Complete Track of update,delete and modified field set.


# Few Important points to be kept in mind is that 
1. default should be used when database is required perform any Operations
2. default = current_timestamp
3. default = current_timestamp

# How to Complete Information of Information Schema in any Database (Table_schema)
SELECT * FROM INFORMATION_SCHEMA.TABLES WHERE TABLE_SCHEMA = 'accountswhol'
SELECT create_time FROM INFORMATION_SCHEMA.TABLES WHERE TABLE_SCHEMA='your_database_name' and Table_name = 'your_table_name';
