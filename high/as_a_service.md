
**MongoDB**   
*E2*   
What:
- one of the most popular NoSQL databases, it is document oriented 
- shuns the traditional relational database schema for JSON like objects 

Strengths:
- supports full indexing - primary and secondary
- huge community of users; tested and ready for production environments
- it is open source and free to use 
- it has a flexible schema - you could even all it schema-less 
- this is a huge value if you are still in the early stages of your use case and you aren't sure how your data is going to be laid out 
- performs better if your application is more read intensive than write 
- there is built in sharding in MongoDB which doesn't exist for MySQL 

Weaknesses:
- by virtue of being document oriented, you lose some functionality that traditional RDBMS has, specifically JOINs 
- there is no current support for transactions 
- not as mature as the traditional RDBMS 
- development is very fast so the system is changing pretty rapidly 

References:
- [1] http://www.mongodb.org/
- [2] http://en.wikipedia.org/wiki/MongoDB
- [3] http://www.sarahmei.com/blog/2013/11/11/why-you-should-never-use-mongodb/
- [4] http://stackoverflow.com/questions/5244437/pros-and-cons-of-mongodb
- [5] http://www.quora.com/What-are-the-pros-and-cons-of-Mongo-DB-compared-to-MySQL-database
- [6] http://www.quora.com/Document-oriented-Databases/Can-someone-weigh-the-pros-and-cons-of-MongoDB-vs-Clusterpoint-software-I-cant-find-much-on-Clusterpoint-as-they-havent-really-penetrated-markets-outside-of-Latvia-yet



**MongoLab**  
*E2*    
What:
- cloud database service that will host MongoDB databases 
- you can think of it as a MongoDb as a service 

Strengths:
- ease of use 
- have a free plan which is good for startups, school projects
- would be great to use for our CS516 final project if we were using MongoDB
- great customer support 

Weaknesses:
- won't be able to support heavy customization 

References:
- [1] https://mongolab.com/
- [2] http://en.wikipedia.org/wiki/MongoLab
- [3] http://mrdanadams.com/2012/mongohq-mongolab-mongodb-customer-service/#.VMV6Xy6Ynxg
- [4] http://webmasters.stackexchange.com/questions/20782/mongodb-hosting-mongolab-vs-mongohq-vs-mongomachine
- [5] http://www.quora.com/What-is-the-best-mongodb-hosting



**Google BigQuery**  
*D5*
What:
- service from Google that allows you to interactively query using a SQL-like interface over massive amounts of data 
- you import all your data into Google 
- the service is built on Google's underlying infrastructure 
- marketed as a more powerful, faster alternative to Hadoop although it can be used in conjuction with it 

Strengths:
- easy to access and use this service 
- Google provides a web UI and a RESTful API 
- performance over Hadoop 

Weaknesses:
- costs money 
- not open source, enterprise 

References:
- [1] https://gavinbadcock.wordpress.com/2013/02/06/googles-bigquery-vs-hadoop-complimentors-or-competitors/
- [2] https://cloud.google.com/bigquery/what-is-bigquery
- [3] http://en.wikipedia.org/wiki/BigQuery
- [4] http://news.dice.com/2013/04/15/googles-bigquery-vs-hadoop-a-matchup-2/
- [5] http://www.megapivot.com/blog/posts/redshift-vs-bigquery-vs-hadoop.html




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




**MySQL**  
*C4*  
What:
- one of the most popular open source RDBMS currently developed by Oracle
- it is used heavily for web development as it is a critical component of the LAMP stack

Strengths:
- learning curve is pretty low compared to Postgres
- getting Postgres configured, creating a user, etc, was a bit of pain
- free to use 
- can run on Linux, which is a draw because that is the operating system of choice for many web servers 

Weaknesses:
- not as mature as other open sourced databases such as PostgreSQL
- development is not community driven but rather driven by Oracle 
- this can actually be a strength though, it depends on whether you value a slower more robust enterprise development
- from a performance standpoint, I've seen people citing that Postgres benchmarks a little better than MySQL but the difference is marginal 

References:
- [1] http://www.mysql.com/
- [2] http://en.wikipedia.org/wiki/MySQL
- [3] http://www.smartfile.com/blog/the-pros-and-cons-of-mysql/
- [4] https://www.digitalocean.com/community/tutorials/sqlite-vs-mysql-vs-postgresql-a-comparison-of-relational-database-management-systems
- [5] http://stackoverflow.com/questions/4779029/why-is-mysql-used-so-often-in-web-development
- [6] http://www.sitepoint.com/forums/showthread.php?34311-Why-is-MySQL-so-popular
- [7] http://www.quora.com/Why-is-MySQL-more-popular-than-PostgreSQL
- [8] http://www.wikivs.com/wiki/MySQL_vs_PostgreSQL




**AWS DynamoDB**   
*E2*  
What:
- NoSQL database service 
- fully managed database that supports document and key value data models 

Strengths:  
- great for lookup queries 
- persistent store unlike Redis which is for temporal data 
- schema free, lightweight 

Weaknesses:  
- join queries 
- good for specific well defined tasks but it seems like it's not full featured enough to be a standalone DB solution to serve your entire system 

References:  
- [1] http://aws.amazon.com/dynamodb/
- [2] http://db-engines.com/en/system/DynamoDB%3BMySQL
- [3] http://www.quora.com/How-does-one-choose-DynamoDB-versus-Redis-ElastiCache-on-AWS



**AWS ElastiCache**   
*E4*  
What: 
- web service for an in memory cache service in the cloud 
- supports the caching engines of memcached, redis 

Strengths:  
- operational abstraction, easier to maintain and set up than putting up your own EC2 and running Redis 
- dynamic allocation of resources 

Weaknesses:  
- expensive: costs 30% more than a normal instance and you need to pay for all the memory for the instance even if you don't use it 

References:  
- [1] http://aws.amazon.com/elasticache/
- [2] http://stackoverflow.com/questions/21175941/redis-amazon-ec2-vs-elasticache
- [3] http://www.quora.com/What-are-the-advantages-and-disadvantages-of-using-AWS-Elasticache-over-self-hosted-Memcached
- [4] http://harish11g.blogspot.in/2012/11/amazon-elasticache-memcached-ec2.html


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



**AWS Redshift**   
*D6*  
What:
- data warehouse solution that makes it easy to do analysis on the data using your own business analytics tools

Strengths:  
- fast query performance from columnar storage 
- offers a wide range of SQL clients: PostgreSQL
- also it's pretty cheap compared to its competitors (unusual for AWS) 

Weaknesses:  
- doesn't have uniqueness so you need to make sure you haven't already written your data to Redshift 
- quite difficult to do ETL 
- doesn't have the features that a competing product like Hive has 

References:  
- [1] http://aws.amazon.com/redshift/
- [2] http://www.quora.com/What-are-some-good-real-world-examples-of-using-Amazon-redshift
- [3] http://www.quora.com/What-are-the-pros-and-cons-of-using-Amazon-Redshift



**Azure DocumentDB**  
*E2*  
What:
- Microsoft's proprietary NoSQL document database 
- DEFN: document oriented databases are used for semi-structured data like scanning a paper document

Strengths:
- natively supports JSON and JavaScript, which makes it an attractive choice for web and mobile heavy applications 
- there is no schema yet you can still use the familiar SQL query syntax 
- performs better on scalability and availability compared to a competitor like MongoDB 

Weaknesses:
- being a commercial product, loses out on the advantages of having an open source community that MongoDB would have 
- one example of that is that it doesn't support as many programming languages as MongoDB (only supports JavaScript, Python, and .NET)

References:
- [1] http://azure.microsoft.com/en-us/services/documentdb/
- [2] http://en.wikipedia.org/wiki/Document-oriented_database
- [3] http://daprlabs.com/blog/blog/2014/08/22/azure-documentdb/
- [4] http://db-engines.com/en/system/Microsoft+Azure+DocumentDB%3BMongoDB



**Azure Search**  
*B2* 
- Microsoft's search as a service platform 
- built on top of Elastisearch, which provides for its text search

Strengths:
- out of the box ease of use; building out a custom search feature for your own company, handling search indices is no trivial task 
- makes scalability very simple especially compared to SOLR which is quite difficult to scale  

Weaknesses:
- expensive 
- commercial and proprietary compared to the open sourced alternative of SOLR  

References: 
- [1] http://azure.microsoft.com/en-us/services/search/
- [2] http://www.tugberkugurlu.com/archive/a-gentle-introduction-to-azure-search
- [3] http://cloudcomputing.sys-con.com/node/3221202
- [4] http://weblogs.asp.net/scottgu/azure-new-documentdb-nosql-service-new-search-service-new-sql-alwayson-vm-template-and-more




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


**Hortonworks**  
*A5*  
What:
- a company that builds a variety of solutions for Hadoop 
- they are main competitors with Cloudera and MapR; the emergence of these enterprise Big Data companies 
- they perform a lot of open source development for Hadoop 
- all of these Hadoop distribution providers make their money by selling a suite of services on top of their software 

Strengths:
- Hortonworks and Cloudera provide nearly 100% open source distributions of Hadoop, something their competitor MapR does not do (they have more proprietary modules)
- these are the guys who came out with YARN which is a new version of Hadoop better than the previous MapReduce; YARN allows the inclusion of more data processing frameworks 

Weaknesses:
- because Hortonworks' distribution is completely open source, it is not as enterprise ready as something like MapR's distribution 
- they don't have the reach of Cloudera, who has been around the longest and has the most number of customers
- this does give Cloudera a bit of an edge in terms of knowing what features are needed 

References:
- [1] http://hortonworks.com/hadoop-modern-data-architecture/
- [2] http://en.wikipedia.org/wiki/Hortonworks
- [3] http://www.experfy.com/blog/cloudera-vs-hortonworks-comparing-hadoop-distributions/
- [4] http://www.quora.com/What-are-some-major-pros-cons-of-Cloudera-vs-Hortonworks-as-a-Hadoop-platform-for-a-main-street-e-g-not-Silicon-Valley-giant-enterprise
- [5] http://www.quora.com/What-distribution-should-I-choose-Cloudera-Hortonworks-or-MapR



**Databricks/Spark**  
*A5*  
What:
- open source processing engine for Hadoop data 
- Spark is now an Apache project but Databricks is a main developer for it

Strengths:
- speed (up to 100x faster in memory, 10x on disk)
- flexibility in that it can use either memory or disk unlike Hadoop which uses HDFS (disk)
- enormous open source community 
- features beyond basic map and reduce: allows for SQL queries, streaming data, machine learning libraries 
- great for iterative processing, interactive processing, and event stream processing ]

Weaknesses:
- pretty young system so still some bugs, not nearly as mature as Hadoop 

References:
- [1] https://databricks.com/spark
- [2] http://en.wikipedia.org/wiki/Apache_Spark
- [3] http://www.quora.com/What-are-the-pros-and-cons-of-Apache-Spark
- [4] http://www.javaworld.com/article/2360185/big-data/straight-talk-on-apache-spark-and-why-you-should-care.html
- [5] http://stackoverflow.com/questions/25267204/hadoop-vs-spark


**AWS EMR**   
*A4*  
What:
- stands for Elastic Mapreduce 
- uses Hadoop to do the data distribution and computation but can also use Spark or Presto

Strengths:  
- the ability to get computation on tap 
- lots of the details are managed for you 
- lowest barrier to usage 

Weaknesses:  
- keeping it running is expensive 
- doesn't have features like automatic cluster lifecycle management, automatically scaling up and down
- known to get unstable at scale 

References: 
- [1] http://aws.amazon.com/elasticmapreduce/
- [2] http://www.quora.com/What-is-your-feedback-of-using-Amazons-EMR-or-Hadoop-on-EC2-or-CDH-for-Telecoms-data-CDR-Recharge-Transactions-others-event-data
- [3] http://engineering.pinterest.com/post/92742371919/powering-big-data-at-pinterest



