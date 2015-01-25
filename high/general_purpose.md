
**AWS RDS**   
*D5*  
What:
- Amazon's version of a traditional relational database in the cloud 
- you can compare it to a self hosted MySQL 

Strengths:  
- comes with all the Amazon managed goodies (backups, patch management, and replication)
- have this feature called multi AZ which stands for multi availability, which handles replication and backups for failure 
- it also gives a very good up time ~99.95% 

Weaknesses:  
- couple drawbacks to RDS when you are doing complex operations that require many privileges 
- doesn't have very high security needs 
 
References:  
- [1] http://aws.amazon.com/rds/
- [2] http://www.laurencegellert.com/2013/05/pros-and-cons-of-rds-vs-ec2-for-mysql-with-aws/
- [3] https://www.scalebase.com/aws-rds-vs-self-hosted-mysql-availability-scalability-performance/


**Azure SQL Database**  
*D5*  
What:
- Microsoft's proprietary relational database as a service 

Strengths:
- similar to many of the AWS products, SQL Database can dynamically scale up to thousands of machines based on load 
- they manage the service for you so you don't need to devote engineering resources to maintenance 
- pretty cheap compared to AWS RDS because Amazon dedicates resources to an individual entity whereas Azure sharees the resources 

Weaknesses:
- size limitations: Azure only allows up to 50GB whereas RDS allows for 1TB 
- doesn't handle data restoration as well as RDS, for Azure you need to manually configure and set up how you want to do backups where RDS just does 8 days of backups automatically for you 
- fewer features than RDS which has the full fledged MySQL feature set 

References: 
- [1] http://azure.microsoft.com/en-us/services/sql-database/
- [2] https://www.develop.com/sqlazurevsamazonrds



**Firebird**  
*B3*  
What:
- open source SQL RDBMS that runs on all major operating systems - Windows, Linux, Unix 
- what you find is that the main differentiators from these RDBMS systems is how they choose to index their data 
- that is what leads to the tradeoffs in performance as certain indexing paradigms are better for certain data sets and operations 

Strengths:
- many of the basic features you would want in a database such as ACID transactions, referential integrity
- apparently there is little to no need for database admins / low maintenance 
- because it runs on many platforms you can avoid being locked into a vendor 
- open source, which should give you flexibility to tinker with it to your use case 

Weaknesses:
- many people looking for a Firebird solution would already be using MySQL and generally people don't want to migrate from what they currently have if what they currently have works 
- MySQL is supported on more platforms
- MySQL has a much larger community 

References:
- [1] http://www.dbforums.com/showthread.php?793966-MySQL-vs-Firebird
- [2] http://www.firebirdsql.org/
- [3] http://en.wikipedia.org/wiki/Firebird_(database_server)
- [4] http://www.firebirdsql.org/manual/migration-mssql-pros-cons.html


