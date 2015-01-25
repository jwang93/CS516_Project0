
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



