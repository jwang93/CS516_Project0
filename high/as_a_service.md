
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



