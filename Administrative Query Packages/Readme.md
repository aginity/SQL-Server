# SQL Server Package Summary

|Package Name| Package Description| Number of Queries in Package|
|------------|--------------------|-----------------------------|
|Aginity-Pro-SQLServer-Admin-Set1 |Contains common SQL queries to better understand SQL Server objects   | 8  |




### The table below details all queries within the [Aginity-Pro-SQL Server-Admin-Set1](https://github.com/aginity/SQL-Server/blob/master/Administrative%20Query%20Packages/Aginity-Pro-SQLServer-Admin-Set1.aginitypkg) package.

|Catalog Item Name               |Catalog Item Description            | Required Table     |
|--------------------------|------------------------------------|--------------------|
|Get Index Usage Statistics for Current Database   | Will give statistics on how indexes on tables are being used    |sys.tables,sys.dm_db_index_usage_stats, sys.indexes   |
|Performance Killer Wait Types Found   | Finds processes that are in wait status which can degrade performance of your SQL Server queries  | sys.dm_os_wait_stats   |
|Performance Statistics for Cached Query Plans   | Shows you detail about the SQL statements that have been cached  | sys.dm_exec_query_stats, sys.dm_exec_sql_text  |
|Show List of Active Process with SQL Text   | What SQL processes are running right now on the SQL Server instance  | sys.dm_exec_requests, sys.dm_exec_sql_text, sys.dm_exec_sessions   |
|Show Sizes for All Databases   | Shows database size in MB  |  sys.master_files, sys.databases |
|Show Unused Tables Since Last Restart   | A great query showing you which tables have not been referenced   |  sys.tables,sys.dm_db_index_usage_stats, sys.indexes  |
|Top 10 Biggest Tables in Database   | Shows which tables are taking up the most space in a database   | sys.dm_db_partition_stats   |
|User Statistics   |Shows current logged in users and a summary of their activity   |sys.dm_exec_sessions sessions, sys.dm_exec_connections, master..sysprocesses requests,sys.dm_exec_cursors   |
