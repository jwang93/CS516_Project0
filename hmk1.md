# CS 516 - Homework 1 
Name: Jay Wang  
NetID: jmw86  
Due Date: Jan 21, 2015
  
    
      
## **Systems**

**1) 1010data**  
*D6*  
What:  
- database with spreadsheet interface
- customers like Clorox, Morgan Stanley
- B2B enterprise company
- replacement to traditional data warehouse  

Strengths:  
- easy to use, don't need deep technical knowledge 
- cloud based so can be accessed anywhere 
- provides clients with industry specific solutions
- NoSQL

Weaknesses:  
- technical portion is heavily abstracted 
- limitations to what a client can do 

References:   
- [1] https://www.1010data.com/products/detail/1010data-industry-specific-applications
- [2] http://www.itworld.com/article/2730562/big-data/1010data--the-non-elephant-in-the-big-data-room.html 

**2) Accumulo**    
*D2*  
What:  
- sorted, distributed key-value store 
- based on Google BigTable 
- built on Hadoop, Zookeeper, and Thrift   

Strengths:  
- high availability 
- sorted and distributed 
- scales well while delivering good performance  

Weaknesses: 
- does not support a "NOT" operator.. for security reasons
- when compared to HBase, Accumulo is less popular and thus has fewer integrations with other systems

References: 
- [1] https://accumulo.apache.org/ 
- [2] http://www.cloudera.com/content/cloudera/en/products-and-services/cdh/accumulo.html
- [3] http://apache-accumulo.1065345.n5.nabble.com/How-does-Accumulo-compare-to-HBase-td10464.html  

**3) Actian Ingres**  
*B3*  
What:  
- database management system
- used for enterprise 
- open source, SQL 

Strengths:  
- has out of the box spatial management  
- traditional database features - ACID, transactions
- open source 

Weaknesses:  
- bit archaic 
- fact that it uses SQL creates a barrier to use 

References:  
- [1] http://www.actian.com/products/operational-databases/ingres/
- [2] https://www.princeton.edu/~achaney/tmve/wiki100k/docs/Ingres_%28database%29.html 

**4) Actian Matrix**  
*C6*  
What:  
- analytics database from Actian

Strengths:  
- comes with many built in algorithms courtesy of Actian
- parallel, columnar, compressed
- compiles queries during query execution which reduces overhead 
- has an option to be run entirely in memory 

Weaknesses:  
- expensive

References:  
- [1] http://wwwcdn.actian.com/wp-content/uploads/2014/01/Actian-Matrix-Datasheet.pdf


**5) Actian PSQL**  
*B5*  
What:
- yet another database management system from Actian

Strengths:  
- has the ability to be embedded making it good for packaged business apps 
- very low maintenance - they call it "Zero DBA"

Weaknesses:  
- expensive 
- limited functionality compared to a more involved system 

References:  
- [1] http://www.actian.com/products/operational-databases/psql/


**6) Actian Vector**  
*C6*  
What:  
- analytical database system 
- successor to MonetDB
- SQL on Hadoop 

Strengths:  
- data partitioning and parallel load feature allow for shorter data loading time 
- performance boosts from compression and better I/O scheduling 

Weaknesses:  
- doesn't really scale out that well 
- expensive 

References:  
- [1] http://www.actian.com/about-us/blog/vectorwise-goes-hadoop/ 
- [2] http://www.actian.com/about-us/blog/pssst-want-hear-actian-vector-3-5/ 
- [3] http://www.dbms2.com/2013/04/25/goodbye-vectorwise-farewell-paraccel/

**7) Actian Versant**   
*E1*  
What:
- object database 
- Actian acquired Versant to expand its data analytics offerings 

Strengths:  
- handling more complex object models 
- NoSQL
- focused on real-time analytics 

Weaknesses:  
- steep technical knowledge required to use

References:  
- [1] http://www.actian.com/products/
- [2] http://globenewswire.com/news-release/2012/11/21/506794/10013391/en/Versant-Agrees-to-be-Acquired-by-Actian-for-13-00-per-Share.html
- [3] http://en.wikipedia.org/wiki/Versant_Object_Database

**8) Adabas**  
*D1*  
What:
- database management system from Software AG
- stands for Adaptable Database System 
- it is NoSQL, not relational 

Strengths:  
- performance (esp. on mainframes) 
- inverted list architecture makes it faster than traditional relational DB's 

Weaknesses:  
- doesn't do data compression or encryption like DB3 does 
- doesn't have the referential integrity that Oracle MySQL has 

References:  
- [1] http://tech.forums.softwareag.com/techjforum/posts/list/24345.page
- [2] http://database-management.findthebest-sw.com/compare/2-9/ADABAS-vs-DB3 
- [3] http://database-management.findthebest-sw.com/compare/2-30/ADABAS-vs-MySQL

**9) Aerospike**  
*C2*  
What:
- optimized for flash, in-memory database
- NoSQL database 

Strengths:  
- flash optimized, so should be super fast with a hybrid RAM/Flash storage architecture
- good for concurrent, low latency, more read than write 

Weaknesses: 
- jobs with high write volume 
- can't operate on non-SSDs which makes it more expensive than something like Cassandra were you can store your keys on disk 

References:  
- [1] http://www.aerospike.com/
- [2] http://www.aerospike.com/about-aerospike/
- [3] http://stackoverflow.com/questions/25443933/comparison-aerospike-vs-cassandra

**10) AffinityDB**   
*E1*  
What: 
- platform for information processing, control
- at its core it is a graph database
- runs something called pathSQL 

Strengths:  

Weaknesses:  
- little information / documentation on affinityDB

References:
- [1] http://affinityng.cfapps.io/doc/terminology.html#pathsql



**11) Allegrograph**  
*E1*  
What:
- specifically a graph database 
- uses combination of memory and disk allowing for huge scale 
- utilizes an RDF store (triple store of the form - subject:predicate:object)

Strengths:  
- huge scale due to its usage of disk 
- has a java client library that supporst Jena and Sesame 
- supports SPARQL queries 

Weaknesses:  
- there are competing graph databases that are open source, Allegro is commercial license
- not embeddable compared to competitor Neo4J 
- doesn't support MapReduce? 

References:  
- [1] http://franz.com/agraph/allegrograph/
- [2] http://db-engines.com/en/system/AllegroGraph%3BNeo4j%3BVoltDB
- [3] http://stackoverflow.com/questions/2613357/difference-between-graph-database-neo4j-allegrograph
- [4] http://vschart.com/compare/allegrograph/vs/neo4j


**12) Altibase HDB**   
*D3*  
What:
- hybrid in memory database, hence the name HDB developed by altibase 
- utilizes spatial indexing 

Strengths:  
- purported to be very fast (although this is from Altibase)
- lot of features that competitors don't have such as - SQL Interpreter, Java Support, Real Time Access

Weaknesses:  

References:  
- [1] http://altibase.com/in-memory-database-hybrid-products/hdbtm-hybrid-dbms/
- [2] http://database-management.findthebest-sw.com/compare/5-36/ALTIBASE-HDB-vs-Oracle 


**13) Altibase XDB**   
*D3*  
What:
- XDB stands for extreme in memory database - memory only 
Strengths:  
- very fast 

Weaknesses:  
- requires a lot of memory 
- can't utilize disk 
- limited operating systems support 

References:  
- [1] http://altibase.com/in-memory-database-hybrid-products/xdb/

**14) Altiscale**  
** I have used Altiscale before at my previous internship at Drawbrdge **  
*A3*  
What:
- company that provides Hadoop cloud services, they run your Hadoop workloads for you 
- notion of Hadoop as a Service 

Strengths:  
- easy to use, configurations all handled for you, customer support 
- cloud nature can handle variability of Hadoop workloads 
 
Weaknesses:  
- expensive - would be much cheaper to roll out your own Hadoop infrastructure 
- less control over your Hadoop jobs than if you ran it yourself 

References:  
- [1] https://www.altiscale.com/why-altiscale/

**15) Apache Drill**   
*B4*  
What:
- open source, SQL query engine for Hadoop and NoSQL
- direct queries on semi-structured data such as JSON with needing to maintain specific schemas 

Strengths:  
- real time data exploration, supposed to be "agile" 
- open source community driven project (can also be a weakness)
- can work on not only Hadoop but also MongoDB, Cassandra, Riak, and Splunk 

Weaknesses:  
- community driven project, makes development a bit more chaotic

References:  
- [1] http://drill.apache.org/
- [2] http://www.quora.com/Isnt-Cloudera-Impala-doing-the-same-job-as-Apache-Drill-incubator-project
- [3] http://gdfm.me/2012/10/27/the-rise-of-the-dremel-clones/
- [4] https://www.mapr.com/products/apache-drill


**16) Apache Hive**   
** I have experience using Hive before **  
*B4*  

What:
- open source data warehouse software 
- initially came from Facebook 
- DEFN: data warehouse: system used for reporting and data analysis   

Strengths:  
- easy to use due to its abstracted SQL-like language called HiveQL
- has flexibility to plug in custom mappers and reduces 

Weaknesses:  
- basic weakness of batch processing is that it is slow
- imposes the relational rigor of a database (ie schema)

References:  
- [1] https://hive.apache.org/
- [2] http://www.quora.com/What-are-the-pros-and-cons-between-Pig-and-Hive
- [3] http://stackoverflow.com/questions/9569009/what-are-the-pros-and-cons-of-running-a-job-in-hadoop-using-various-languages

**17) Apache S4**  
*A2*  
What:
- made more for processing continuous streams of data (real time data ingestion)
- can be compared to Twitter Storm 

Strengths:  
- good for stream/real-time applications (don't want to do batch)
- data is optimized for a stream 
- modular and pluggable: many of the components can be replaced on developer discretion

Weaknesses:  
- data reliability 
- apparently it's quite buggy? 

References:  
- [1] http://incubator.apache.org/s4/ 
- [2] http://www.quora.com/How-does-S4-compare-to-Flume
- [3] http://www.quora.com/What-would-you-choose-between-Flume-Yahoo-S4-and-Backtype-Twitter-Storm-and-why

**18) Apache Storm**   
*A2*   
What:
- distributed realtime computation system initially developed out of Twitter
- trying to do for realtime processing what Hadoop did for batch 
- operates on data in motion, not data at rest 

Strengths:  
- the spout abstraction makes it easy to integrate with a number of queuing and database systems 
- great for low latency results and no data loss 
- widely used with a large and active community 

Weaknesses:  
- narrow in that it only allows for one type of input - the stream 
- doesn't support exactly-once processing, may perform duplicate processing called "at least once processing"

References:  
- [1] https://storm.apache.org/ 
- [2] http://www.quora.com/What-is-the-difference-between-Apache-Storm-and-Apache-Spark
- [3] http://xinhstechblog.blogspot.co.uk/2014/06/storm-vs-spark-streaming-side-by-side.html
- [4] http://stackoverflow.com/questions/15520993/storm-vs-trident-when-not-to-use-trident

**19) Apache Tajo**   
*B3*  
What:
- relational, distributed data warehouse system built on Hadoop 
- SQL query processing engine 
- one of the growing number of SQL-on-Hadoop frameworks 

Strengths:  
- can adjust query processing based on: user queries, characteristics of data, cluster status
- supports SQL standards which gives it a lower barrier to entry 
- great performance (way better than Hive) and better than Impala on: filters, group by, join, filter scan 

Weaknesses:  
- worse than Impala when you do a union and then join
- smaller community as it is developed in Korea may not make it worth it when you have really good alternatives in Impala and Presto 

References:  
- [1] http://mail-archives.apache.org/mod_mbox/tajo-dev/201305.mbox/%3CCACZfFK6PNE+AuNX6CQ0WD784ZxUavEykEKa-rWFMXp0xdyAHmg@mail.gmail.com%3E
- [2] http://tajo.apache.org/
- [3] http://blogs.gartner.com/nick-heudecker/apache-tajo-enters-the-sql-on-hadoop-space/
- [4] http://blog.matthewrathbone.com/2014/06/08/sql-engines-for-hadoop.html#apache-tajotajo

**20) ArangoDB**   
*B2*  
What: 
- open source, NoSQL database 
- multi model database 

Strengths:  
- great for documents, graphs, and key values
- supports a SQL like query language making it easy to use
- supports some JavaScript extensions 
- multi model database allows for different data models (graphs and documents) in the same application that might even need to be mixed in the same query 

Weaknesses:  
- not embeddable like its competitor OrientDB 
- the restriction on the max value size is 256MB compared to 2GB for a competitor 

References:  
- [1] https://www.arangodb.com/
- [2] http://vschart.com/compare/arangodb/vs/orientdb
- [3] http://stackoverflow.com/questions/26704134/mongodb-neo4j-vs-orientdb-vs-arangodb


**21) Attivio**   
*A1*  
What:
- working on enterprise search and discovery 
- enterprise software company that sells a platform that lets users find all types of information from a single query 
- based off Lucene 

Strengths:  
- giving traditional enterprise search engines database features such as joins 
- bridging a lot of previously disparate entities into one: enterprise search, BI, data warehousing, analytics 

Weaknesses:  
- proprietary and not open source, lots of commercial licenses 
 
References:  
- [1] http://en.wikipedia.org/wiki/Attivio
- [2] http://www.cominvent.com/2009/02/11/attivio-promises-to-bridge-the-gap/
- [3] http://www.realstorygroup.com/Blog/1294-How-Fast-is-Attivio

**22) AWS DynamoDB**   
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

**23) AWS ElastiCache**   
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

**24) AWS ElastiCache with Redis**  
*E2*  
What: 
- same thing as ElastiCache, just that you are using Redis rather than Memcached as the memory caching service 

Strengths: 
- get the same abstraction of not having to manually set up Redis 

Weaknesses:  
- cost 

References:  
- [1] http://aws.amazon.com/elasticache/
- [2] http://stackoverflow.com/questions/21175941/redis-amazon-ec2-vs-elasticache

**25) AWS EMR**   
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


**26) AWS Kinesis**  
*A2*  
What: 
- fully managed cloud based service for realtime processing of large data streams (think competitor to Kafka, Spark Streaming)

Strengths:  
- like most of these AWS services (called managed services), it is very easy to set up and get started
- elasticity allows for easy scaling 

Weaknesses:  
- software as a service means you will need to pay money, which sucks because there are open source alternatives such as Kafka 
- every application consists of just one procedure so you can't do complex stream processing like in Storm 

References:  
- [1] http://aws.amazon.com/kinesis/
- [2] http://www.quora.com/What-can-you-do-with-Amazon-Kinesis
- [3] http://gworley3.blogspot.com/2013/11/amazon-kinesis-compared-to-storm.html
- [4] http://diamondstream.com/amazon-kinesis-big-real-time-data-processing-solution/

**27) AWS RDS**   
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

**28) AWS Redshift**   
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

**29) AWS SimpleDB**  
*E2*  
What:
- Amazon's non relational data store 

Strengths:  
- managed multiple copies of your data in various geographic locations which helps to ensure reliability 
- simplicity that comes from not being a relational database: don't have to worry about schema and adhering to strict rules 
- cheap set up costs and the ability to pay as you go makes it ideal for startups 

Weaknesses:  
- missing a couple of standard SQL operators like JOIN or IN 
- relatively high cost given how easy it is to set up a standalone DB
- your data is under Amazon which can potentially lead to privacy issues (note that this is the case for all of these AWS services)

References:  
- [1] http://highscalability.com/current-pros-and-cons-list-simpledb
- [2] http://aws.amazon.com/simpledb/


**30) Azure DocumentDB**  
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


**31) Azure Search**  
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

**32) Azure SQL Database**  
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

**33) BerkeleyDB**  
*D2*  
What:
- produced by Oracle, claiming to be an open source and embeddable storage engine 
- it is a key value store database (also relational) with low administration 

Strengths:
- very easy to manage 
- flexibility in managing databases in memory, disk or both 
- decent performance, about 65% faster than MySQL because it does not deal with IPC 

Weakness:
- weak community support
- limited feature set in the sense that it doesn't support mapreduce, server side scripts, foreign keys, partitioning 

References:
- [1] http://www.oracle.com/technetwork/database/database-technologies/berkeleydb/overview/index-085366.html
- [2] http://vschart.com/compare/berkeley-db/vs/mysql
- [3] http://db-engines.com/en/system/Berkeley+DB%3BMongoDB
- [4] http://perfectmarket.com/nosql-solution-evaluation-and-comparison-mongodb-vs-redis-tokyo-cabinet-and-berkeley-db-chart/
- [5] http://blog.cppcms.com/post/8

**34) BigCache**  
*E4*  
- caching API developed by Google that is backed on Amazon S3
- could hardly find any information about BigCache 

Strengths:
- very simple to use 
- can support asynchronous methods 
- a double layer cache that makes use of your unused disk memory 
- first layer is in memory and disk caching, second layer is S3

Weaknesses:
- little popularity, almost no community/discussion about it even though it is open sourced 
- looks very cool and easy to use, so I must imagine that there isn't much demand for it, perhaps it only serves a niche use case?

References:
- [1] https://code.google.com/p/bigcache/
- [2] http://java.dzone.com/announcements/bigcache-open-source-heap

**35) BigMemory**  
*E4*  
What:
- can describe this as the data grid and caching market 
- idea is that you can store data off the heap in memory buffers that allows you to avoid garbage collection overhead 

Strengths:
- good to use if you already use Ehcache, as this is what BigMemory was built for 
- performance is very predictable 
- use it if you need very fast performance and can't utilize disk for your business needs

Weakness:
- a memory only product
- therefore, expensive because if you can't afford all that RAM, you can't really use BigMemory

References:
- [1] http://terracotta.org/products/bigmemory
- [2] http://stackoverflow.com/questions/5621209/ehcache-with-terracotta-vs-infinispan
- [3] http://blog.c2b2.co.uk/2013/02/big-memory-under-radar.html
- [4] http://www.softwareag.com/corporate/products/terracotta/in-memory_data_mgmt/overview/default.asp


**36) BitYota**  
*D6*  
What:
- tagline of "Data Warehouse as a service"
- ingest data from a number of sources and perform analysis 

Strengths:
- easy to set up and maintain as it is managed for you 
- supports standard ANSI SQL for a low learning curve 
- focused on taking advantage of being natively on cloud 

Weaknesses:
- as with every data warehouse, they are expensive 
- competes with Redshift which is more widely used and better documented 

References:
- [1] http://www.bityota.com/product/
- [2] http://www.esg-global.com/blogs/the-week-that-waas-bityota-and-redshift/
- [3] http://www.businessinsider.com/bityota-amazon-data-warehouse-2012-11
- [4] http://cloudcomputingeurope.sys-con.com/node/2466082

**37) Cassandra**  
*C2*  
What:
- open sourced, distributed database management system that is unique in that it offers column indexes 
- it is a NoSQL system initially developed at Facebook 
- NoSQL can never replace the relational model (which comes with stuff like ad-hoc queries) but NoSQL will become popular becaues of scale, flexibility, ease of use 
- DEFN ad hoc query: query on the fly where you have some variables that can change value each time the query is executed making it different 

Strengths:
- very popular and under active development with a robust community 
- built for being the best distributed and scalable system while delivering great performance 
- decentralized system means that there is no single point of failure making it rather robust (every node has the same job)

Weaknesses:
- there is no notion of referential integrity which means that you can't perform JOINs
- DEFN referential integrity: data property that requires that every value of one column in a table to exist in a different column in the same table 

References: 
- [1] http://cassandra.apache.org/ 
- [2] http://en.wikipedia.org/wiki/Apache_Cassandra
- [3] http://marsmedia.info/en/cassandra-pros-cons-and-model.php
- [4] http://en.wikipedia.org/wiki/Referential_integrity
- [5] http://stackoverflow.com/questions/2460954/what-is-ad-hoc-query

**38) Cassandra.io**  
*D2*  
What:
- a hosted and managed instance of Cassandra that is made accessible via a RESTful API 

Strengths:
- makes Cassandra even easier to use, especially for any kind of web programming that could utilize an API 
- on the data platforms chart, Cassandra.io sits on the "as a service" category which makes sense 

Weaknesses:
- the additional level of abstraction doesn't give developers as much flexibility as if they used a manually configured standalone Cassandra instance 

References:
- [1] https://bighadoop.wordpress.com/2012/09/09/heroku-and-cassandra-cassandra-io-restful-apis/

**39) CitusDB**  
*B5*  
What:
- database system focused on scaling out PostgreSQL
- done via sharding and replication 

Strengths:
- supports semi structured data over JSON and log files 
- strong performance numbers, seems to perform slightly better than Impala in some benchmarks
- PostgreSQL at the core which is an incredibly popular open sourced database with many features

Weaknesses: 
- read a blog that stated that CitusDB was really fast for some basic benchmarks 
- however when he wanted to run complex queries - utilizing distinct and subqueries - CitusDB didn't work and he had to change to Redshift 

References:
- [1] http://haifzhan.blogspot.com/2014/03/citusdb-experience.html
- [2] http://www.quora.com/How-does-CitusDB-compare-to-Cloudera-Impala
- [3] http://www.citusdata.com/blog/86-making-postgresql-scale-hadoop-style


**40) ClearDB**  
*D5*  
What:
- database for MySQL applications 
- impressive customer set of Microsoft and salesforce 

Strengths:
- fault tolerant, which means that if a component fails, a backup system can come back up immediately with no need for human maintenance 
- can support database size up to 10GB 

Weaknesses:
- doesn't have the community of Amazon RDS 
- easy to set up (< 1 minute) but you need to use one of their partners: Heroku, Appfog, Azure cloud 

References:
- [1] https://www.cleardb.com/
- [2] http://w3facility.org/question/xeround-vs-cleardb-hosted-mysql-pros-and-cons/
- [3] http://www.sitepoint.com/database-as-a-service-mysql-in-the-cloud/


**41) Cloudant**  
*E2*  
What:
- fully managed NoSQL Database as a service 
- acquired and now managed by IBM 
- ** NoSQL DBs can't do joins the way a relational database does, NoSQL DB is really good for document stores **

Strengths:
- requires no configuration / easy set up
- embeddable, easy to use alongside ElasticSearch
- scales better than MongoDB and more stable 
- queries in JavaScript and REST

Weaknesses:
- can't perform joins (and other downsides of NoSQL)
- expensive 

References:
- [1] https://cloudant.com/
- [2] http://en.wikipedia.org/wiki/Cloudant
- [3] http://blog.postmarkapp.com/post/37338222496/bye-mongodb-hello-cloudant
- [4] http://vschart.com/compare/cloudant/vs/dynamo-db
- [5] https://getsatisfaction.com/application_craft/topics/anyone_have_experience_with_cloudant_couchdb


**42) CloudBird**  
*D2*  
What:
- RavenDB in the cloud

Strengths:
- RavenDB is built for .NET programming (can also support Java and HTML)
- schema free, scalable, transactional 
- good for OLTP (fast, datatore feel)

Weaknesses:
- limited language support results in limited features 
- not a database as a service means that you need to manually configure it yourself 

References:
- [1] http://ravendb.net/
- [2] http://db-engines.com/en/system/MongoDB%3BRavenDB
- [3] http://ayende.com/blog/136196/when-should-you-use-ravendb

**43) Cloudera**  
*A5*  
What:
- multi billion dollar company that provides Hadoop based software and services
- products include: CDH (cloudera distributed hadoop), Spark , Impala, Search

Strengths:
- rather than wade through the many versions of Hadoop and tools associated with it, CDH is a neatly packaged and documented bundle of all Hadoop + Hadoop related tools to make for a more enjoyable development experience 
- some of Cloudera's solutions have been around longer and are more mature than its competitor's solution Hortonworks 

Weaknesses:
- Cloudera's services are expensive (you can download CDH for free but it won't have any technical support or Cloudera manager)
- selling commerical software on top of its open sourced distribution 

References:
- [1] http://www.cloudera.com/content/cloudera/en/products-and-services/cdh.html
- [2] http://en.wikipedia.org/wiki/Cloudera
- [3] http://www.quora.com/Can-someone-provide-comparative-analysis-of-Cloudera-and-Hortonworks
- [4] http://www.b-eye-network.com/blogs/eckerson/archives/2014/02/the_battle_for.php

**44) CloudTran**  
*E5*  
What:
-transaction management product which gives transactions running in distributed or cloud based environments ACID properties
- ACID is atomic, consistent, isolated, durable 
- difference between in memory database and in memory data grid? 
- data grid provides for more scalability yet it requires change to the application 

Strengths:
- built for the cloud so it allows traditional IT departments to migrate their data to the cloud and still have ACID properties 
- allows for in memory data grids to be used for transaction processing 

Weaknesses:

References:
- [1] http://www.cloudtran.com/about.php
- [2] http://en.wikipedia.org/wiki/CloudTran
- [3] http://en.wikipedia.org/wiki/ACID#Atomicity
- [4] http://www.gridgain.com/in-memory-database-vs-in-memory-data-grid-revisited/

**45) Clusrix**  
*C4*  
What:
- ecommerce databaes good for online retailers
- calling itself a "NewSQL database"
- RDBMS systems that are trying to provide the scale of these NoSQL systems while still guaranteeing the great properties of RDBMS like ACID 
- relational database that can scale horizontally as you add more servers 

Strengths:
- scaling transactions, don't want customers to worry about whether their relational database can keep up 
- real time analytics 
- ACID 
- easy to migrate from MySQL to Clustrix 

Weaknesses:
- cost 

References:
- [1] http://www.clustrix.com/
- [2] http://en.wikipedia.org/wiki/Clustrix
- [3] http://blog.clustrix.com/2012/12/11/what-does-it-mean-to-say-clustrix-is-a-mysql-replacement/


**46) CockroachDB**  
*C3*  
What:
- transactional geo-replicated data store 
- DEFN: geo-replication is when you keep multiple copies of the data in various geographical locations to speed up the response times of queries 

Strengths:
- very resilient (why it's called CockroachDB), supposed to never fail 
- if one server goes down, another one will be available 
- built for scalability, transactionability, availability 

Weaknesses:
- with all this focus on availability and resiliency, there is probably a performance hit 

References:
- [1] http://cockroachdb.org/
- [2] https://news.ycombinator.com/item?id=7823076
- [3] http://www.quora.com/What-are-some-good-uses-for-CockroachDB-the-open-source-implementation-of-Google-Spanner
- [4] http://www.wired.com/2014/07/cockroachdb/

**47) CodeFutures**  
*C4*  
What:
- big data company that has a suite of products
- focus is on database sharding, product called dBshards 
- have another product called Firestorm which is used for DAO (database access object) 

Strengths:
- providing the benefits of sharding (splitting data across multiple data centers) with little effort
- CodeFutures empowers traditional MySQL databases to do Big Data by allowing to shard the data 

Weaknesses:
- data is partitioned not at the application level (some such as Adam D'Angelo view as bad) 

References: 
- [1] http://en.wikipedia.org/wiki/CodeFutures
- [2] http://codefutures.com/codefutures-blog/
- [3] http://www.quora.com/How-can-MySQL-be-used-for-big-data-analysis
- [4] http://www.quora.com/What-kind-of-layer-should-there-be-between-the-application-level-and-the-database-level-in-order-to-scale-out


**48) Compose**  
*D2*  
What:
- company that offers production ready, cloud hosted services for: mongodb, elasticsearch, redis, postgresql 

Strengths:
- made for developers who don't want to invest time in setting up their own services 
- offers a cloud based solution, so don't need to worry about managing the hardware
- these people are professionals and know exactly how to manage your data 

Weaknesses:
- costs money 

References:
- [1] https://www.compose.io/
- [2] http://www.quora.com/As-a-website-developer-should-i-manage-database-myself-or-give-control-of-this-important-piece-of-my-website-to-someone-else-who-in-fact-is-just-another-startup-MongoHQ-compose-io-Note-I-have-been-playing-around-with-MongoDb-and-really-liked-using-it-but-Im-not-a-master-of-this-domain


**49) Continuent**  
*D4*  
What:
- provide services for database clustering and replication
- DEFN: clustering is when you have several servers connect to a single database
- allows for fault tolerance if one server were to fail
- load balancing, sending the user to the server with lowest load 

Strengths:
- managed for you 
- replication and recovery 
- allows for fault tolerance if one server were to fail
- load balancing, sending the user to the server with lowest load 

Weaknesses:
- pretty lackluster community
- couldn't find much research on it 

References:
- [1] http://www.continuent.com/solutions
- [2] http://www.techopedia.com/definition/17/clustering-databases
- [3] http://www.quora.com/Is-MySQL-Proxy-ready-for-production-use

**50) CortexDB**  
*B2*  
What:
- NoSQL database technology that is schema-less

Strengths:
- temporal database, meaning that it understands time for transactions
- security system
- distributed

Weaknesses:

References:
- [1] http://www.odbms.org/wp-content/uploads/2014/04/CortexDB.pdf
- [2] http://www.odbms.org/2014/04/cortexdb/


**51) Couchbase**  
*C2*  
What:
- NoSQL document oriented database great for applications that are interactive 

Strengths:
- handle many concurrent users 
- scales up with low latency and high throughput 
- based on memcache which is proven to be super fast (hard to get better performance than Couchbase)

Weaknesses:
- fewer querying and indexing options compared to competitor MongoDB 
- doesn't have good dynamic query support compared to Mongo

References:
- [1] http://www.couchbase.com/nosql-resources/what-is-no-sql
- [2] http://en.wikipedia.org/wiki/Couchbase_Server
- [3] http://www.infoworld.com/article/2613970/nosql/nosql-showdown--mongodb-vs--couchbase.html
- [4] http://www.quora.com/How-does-Riak-compare-to-Couchbase

**52) CouchDB**  
*D2*  
What:
- open sourced database focused on being great for the web

Strengths:
- great for the web because it uses JSON to store data
- uses JavaScript as the query language, which uses MapReduce
- HTTP is the API 
- implements MVCC to avoid the need to lock the databases during write operations 

Weaknesses:
- handling data that is always changing 
- doesn't support indexes
- not as good querying support as MongoDB 
- doesn't have the performance MongoDB has 

References:
- [1] http://en.wikipedia.org/wiki/CouchDB
- [2] http://stackoverflow.com/questions/12437790/when-to-use-couchdb-over-mongodb-and-vice-versa
- [3] http://www.quora.com/How-does-MongoDB-compare-to-CouchDB-What-are-the-advantages-and-disadvantages-of-each
- [4] http://nosql.mypopescu.com/post/298557551/couchdb-vs-mongodb


**53) Database.com**  
*D5*  
What:
- cloud database run by Salesforce
- opening up the database it uses to power Salesforce CRM and providing developer tools on top of that 

Strengths:
- many of the similar advantages one gets with AWS 
- seems to be a similar product to the Oracle database but cheaper 
- great for the smaller applicationd developers, mobile developers who are willing to try something new 

Weaknesses:
- security, do you want to hand over your data to another third party?
- lose complete control over your data from a mangement perspective 

References:
- [1] http://www.salesforce.com/platform/database/?d=70130000000lll1
- [2] http://www.quora.com/What-are-the-pros-cons-of-hosting-a-database-on-Salesforces-Database-com-vs-Amazons-Relational-Database-Service
- [3] http://www.infoworld.com/article/2624989/cloud-computing/what-salesforce-s-database-com-really-means.html

**54) Databricks/Spark**  
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

**55) DataStax Enterprise**  
*C2*  
What:
- platform built on Apache Cassandra for analytics for online database applications 

Strengths:
- DataStax basically provides Apache Cassandra but with a bunch of tools and features on top on Apache Cassandra
- easy to set up and maintain 

Weaknesses:
- costs money whereas vanilla Cassandra is free 

References:
- [1] http://www.datastax.com/what-we-offer/products-services/datastax-enterprise
- [2] http://stackoverflow.com/questions/24564725/apache-cassandra-vs-datastax-cassandra


**56) DataTorrent**  
*A2*  
What:
- realtime streaming platform for enterprise 
- similar to Apache Storm 

Strengths:
- handle realtime processing 
- can support "exactly onces" semantics which is when you process the data only once (a problem that a lot of realtime systems have)
- can support a number of data sources 
- runtime operations are managed for you: scaling, resource optimization, availability, etc 

Weaknesses:
- enterprise product you will have to pay for 
- not that much of a community around it (probably not needed since all the maintenance and setup is handled for you) 

References:
- [1] https://www.datatorrent.com/
- [2] http://www.datanami.com/2014/04/23/crossing_the_big_data_stream_with_datatorrent/
- [3] http://hortonworks.com/partner/datatorrent/
- [4] https://mybigdatajourney.wordpress.com/2014/07/24/open-source-storm-vs-commercially-available-data-torrent/

**57) Datomic**  
*C3*  
What:
- transactional, cloud-ready, distributed database 
- implement Datalog 

Strengths:
- kind of like a hybrid between NoSQL and SQL systems
- so you get a minimal schema while still allowing for Joins 
- comes with enterprise support 

Weaknesses:
- doesn't provide all the benefits of a NoSQL system like the schema-less document object storage model of MongoDB

References:
- [1] http://www.datomic.com/rationale.html
- [2] http://en.wikipedia.org/wiki/Datomic
- [3] http://comments.gmane.org/gmane.comp.db.datomic.user/9

**58) DeepDB**  
*D4*  
What:
- branded as a general purpose database for big data 

Strengths:
- built to provide good performance while scaling up 
- done through writing indexes quickly 
- good for OLTP 
- can perform realtime ACID transactions (similar to that of a normal relational database) and analytics on the same data set 

Weaknesses:
- tough to sell a new type of databae to enterprise customers who prefer to continue using what they have 
- "keep on using something until it breaks"
- introduces a new product in an already very mature and congested space 
- limited community, not much readily available information on it

References:
- [1] http://deep.is/deepdb/
- [2] http://www.dbms2.com/2013/04/14/deep-information-sciences-deepdb/
- [3] http://www.severalnines.com/news/article/database-clustering/is-deepdb-a-good-general-purpose-choice-for-big-data-needs/801612841

**59) Documentum xDB**  
*C1*  
What:
- database out of EMC, interesting because it is a native XML database 
- not relational 

Strengths:
- many of the pros of NoSQL systems such as being able to store more complex objects
- good at managing XML structures
- native XML means that the underlying data is stored as XML so it does not need to convert from XML to a different data type
- this increases efficiency and improves performance 

Weaknesses:
- very niche use case of only XML
- peoeple are moving away from XML because it is too verbose and picking formats such as JSON 

References:
- [1] http://www.emc.com/products/detail/software2/documentum-xdb.htm
- [2] http://en.wikipedia.org/wiki/XML_database

**60) Drizzle**  
*C4*  
What:
- open source cloud RDBMS forked off MySQL 
- moved all the non essential components of MySQL out into modules that can be added independently 

Strengths:
- supposed to be a trimmed down version of MySQL
- this should give it a performance boost 
- cache and optimization components more pluggable than MySQL 
- supposed to be designed for web applications and cloud computing 
- free

Weaknesses:
- project is kind of dead right now, last stable release was 2 years ago
- not well supported
- competitor MySQL works fine for most use cases 

References:
- [1] http://www.drizzle.org/
- [2] http://en.wikipedia.org/wiki/Drizzle_(database_server)
- [3] http://db-engines.com/en/system/Drizzle%3BMySQL
- [4] http://www.linuxuser.co.uk/news/mysql-successor-drizzle-reaches-maturity
- [5] http://www.quora.com/Why-is-Drizzle-dead

**61) Ehcache**  
*E5*  
What:
- basic memory cache used a lot by Java programs developed by Terracotta 

Strength:
- supports both memory and disk stores 
- scales up well 
- fast recovery from outages 
- very fast performance (better than memcached) because it runs in the same JVM process as the application (this is not the case for something like redis 

Weaknesses:
- doesn't support as many native clients as Memcached, which has clients in all major languages 
- ties you to the JVM 

References:
- [1] http://ehcache.org/
- [2] http://en.wikipedia.org/wiki/Ehcache
- [3] http://www.quora.com/Distributed-Caching/Memcached-vs-Ehcached-Which-is-better-and-why
- [4] http://stackoverflow.com/questions/18910822/why-is-ehcache-faster-than-memcache

**62) Elasticsearch**  
*A1*  
What:
- they have something called an ELK stack of Elasticsearch, Logstash, and Kibana 
- get actionable insight in realtime from structured and unstructured data 
- it's a realtime search and analytics engine 
- can also serve the purpose of a schema-less datastore - something like MongoDB 

Strengths:
- has a RESTful web interface (makes it flexible and usable by many people)
- utilizes schema-free JSON documents 
- open source under an Apache License 
- supposed to have a better distributed model and easier to use than SOLR 

Weaknesses:
- less mature and widely used than Solr, mostly because Solr has been around longer 
- no security whatsoever (authentication or access control)
- no support for transactions or data processing

References:
- [1] http://www.elasticsearch.org/overview/
- [2] http://en.wikipedia.org/wiki/Elasticsearch
- [3] http://stackoverflow.com/questions/10213009/solr-vs-elasticsearch
- [4] http://www.quora.com/Why-should-I-NOT-use-ElasticSearch-as-my-primary-datastore

**63) EnterpriseDB**  
*B3*  
What:
- enterprise software, solutions, tools for PostgreSQL 

Strengths:
- supports Postgres which has its own slew of advantages over MySQL 
- comes with a bunch of services like consulting, data management
- more features for enterprise systems are in Postgres 

Weaknesses:
- supports a unique use case of PostgreSQL 
- makes it harder for people using MySQL systems to migrate
- costs money 

References:
- [1] http://www.enterprisedb.com/
- [2] http://en.wikipedia.org/wiki/EnterpriseDB
- [3] http://www.enterprisedb.com/solutions/mysql-vs-postgresql/why-move-mysql-postgres-plus


**64) Exasol**
*C5*

**65) FairCom**
*C3*

**66) FatDB**
*C2*

**67) FathomDB**
*D5*

**68) FeedZai**
*A2*

**69) Firebird**
*B3*

**70) FlockDB**
*D1*

**71) FoundationDB**
*C2*

**72) Galera**
*D4*

**73) GenieDB**
*C4*

**74) Gigaspaces XAP**
*E4*

**75) Giraph**
*E1*

**76) Google BigQuery**
*D5*

**77) Google App Engine Datastore**
*D2*

**78) Google Cloud Dataflow**
*A2*

**79) Google Cloud Datastore**
*D2*

**80) Google Cloud SQL**
*C5*

**81) Google Compute Engine**
*A4*

**82) GrapheneDB**
*D1*

**83) GridGain**
*E3*

**84) Guavus**
*A2*

**85) Hadapt**
*B5*

**86) Handlersocket**
*C2*

**87) Hazelcast**
*E5*

**88) HBase**
*C2*

**89) Heroku Postgres**
*C5*

**90) Hortonworks**
*A5*

**91) HP Autonomy**
*A1*

**92) HP Cloud RDB for MySQL**
*D5*

**93) HP Vertica**
*C6*




































































