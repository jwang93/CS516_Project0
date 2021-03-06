**SQLite**  
*B3*  
What:
- popular lightweight SQL database engine 
- it is a part of the program that is using it
- it is not standalone, which makes it light
- connotation that SQLite is only good for testing and development 

Strengths:
- it is severless and has no configuration making it easy to set up and maintain 
- also get spretty good performance from a speed standpoint because it is completely internal 
- great for testing and development because it's super easy to set up
- good for emebedding inside of an application 

Weaknesses:
- still not your most powerful, robust production databse 
- doesn't have full concurrency in that it can only support one write at a time 
- data amount limitation of 140TB, which is a lot but won't work for some 

References:
- [1] http://www.sqlite.org/
- [2] http://en.wikipedia.org/wiki/SQLite
- [3] https://www.digitalocean.com/community/tutorials/how-and-when-to-use-sqlite
- [4] http://stackoverflow.com/questions/3630/sqlite-vs-mysql


**IBM DB2**  
*C4*  
What:
- family of database servers released by IBM dating back to the 1980s 
- traditionally have supported the relational model
- however, in recent years to meet the new demand, they have experimented with document oriented models are well 

Strengths:
- DB2 is more of an enterprise product although there are many enterprises that use open sourced products like MySQL
- being enterprise and more mature comes with a standard suite of features like disaster recovery, high availability, scaling 
- can store XML natively and retrieve them using xPath, xQuery 

Weaknesses:
- if you are looking for something simpler there are better options such as MySQL
- like every enterprise product, will cost you money, which is unattractive especially when there are free alternatives 

References:
- [1] http://www-01.ibm.com/software/data/db2/
- [2] http://en.wikipedia.org/wiki/IBM_DB2
- [3] http://www.ehow.com/info_12106599_advantages-db2.html
- [4] http://db-engines.com/en/system/DB2%3BMySQL
- [5] http://stackoverflow.com/questions/9299127/mysql-vs-db2-rdbms




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


