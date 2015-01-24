# CS 516 - Homework 1 
Name: Jay Wang  
NetID: jmw86  
Due Date: Jan 21, 2015
  
    
      
## **Main Systems**

**Given that I only have so much time, these are the systems that I focused on**
My criteria for choosing these systems were:
- widely used in industry 
- ample reviews, documentation 
- known for being a forerunner for its class 
- referenced widely
- compared against frequently 


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


**88) HBase**  
*C2*  
What:
- open source, non-relational distributed database that was modeled after Google's BigTable 
- runs of top of HDFS meaning that it interfaces well with Hadoop 
- DEFN: Bloom Filter: probabilistic data structure that can determine whether an element exists in a set 
- HBase is column oriented and well suited for sparse data sets 
- from an architecture standpoint, HBase is more centralized with a master that watches over a bunch of worker nodes; Cassandra is more decentralized where any node can do any operation 

Strengths:
- good for storing large quantities of sparse data 
- an example would be you have billions of records, but only care about the top 5 or so 
- has a feature for Bloom filters, which is what Professor Babu mentioned in class 
- has a native Java API, using Java is a huge plus for some because there are a ton of libraries in Java

Weaknesses:
- doesn't have support for SQL, which is the de facto standard 
- its similar counterpart - Cassandra - does have support for something called CQL (cassandra query language) which is modeled after SQL
- if you must continue using SQL, this weakness ofr HBase may push the direction in favor of Cassandra
- like Cassandra, there is no real support for transactions 
- much weaker documentation compared to Cassandra 

References:
- [1] http://hbase.apache.org/
- [2] http://en.wikipedia.org/wiki/Apache_HBase
- [3] http://en.wikipedia.org/wiki/Bloom_filter
- [4] http://www-01.ibm.com/software/data/infosphere/hadoop/hbase/
- [5] http://www.infoworld.com/article/2610656/database/big-data-showdown--cassandra-vs--hbase.html?page=3
- [6] http://bigdatanoob.blogspot.com/2012/11/hbase-vs-cassandra.html
- [7] http://www.quora.com/What-are-the-differences-between-HBase-and-Cassendra

**90) Hortonworks**  
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





