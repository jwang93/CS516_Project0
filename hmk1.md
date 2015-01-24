# CS 516 - Homework 1 
Name: Jay Wang  
NetID: jmw86  
Due Date: Jan 21, 2015
  
    
      
## **Systems**

**1010data**  
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

**Accumulo**    
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

**Actian Ingres**  
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

**Actian Matrix**  
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


**Actian PSQL**  
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


**Actian Vector**  
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

**Actian Versant**   
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

**Adabas**  
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

**Aerospike**  
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

**AffinityDB**   
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


**Altibase HDB**   
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


**Altibase XDB**   
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

**ArangoDB**   
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


**Attivio**   
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

**AWS ElastiCache with Redis**  
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


**AWS Kinesis**  
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

**AWS SimpleDB**  
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



**BerkeleyDB**  
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

**BigCache**  
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

**BigMemory**  
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


**BitYota**  
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


**Cassandra.io**  
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

**CitusDB**  
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


**ClearDB**  
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


**Cloudant**  
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


**CloudBird**  
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

**CloudTran**  
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

**Clusrix**  
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


**CockroachDB**  
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

**CodeFutures**  
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


**Compose**  
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


**Continuent**  
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

**CortexDB**  
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



**Database.com**  
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

**DataStax Enterprise**  
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


**DataTorrent**  
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

**Datomic**  
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

**DeepDB**  
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

**Documentum xDB**  
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

**Drizzle**  
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

**EnterpriseDB**  
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


**Exasol**  
*C5*  
What:
- database management software company with the primary product of EXASolution 
- in memory, column oriented, relational database management software 
- compresses data heavily 

Strengths:
- doesn't need to be configured/tuned as the database performs self optimization 
- known for really good performance from the columnar orientation + in memory compression 
- perks of column based databases is that you can avoid the need for entire table scans and pre aggregation of data 

Weaknesses:
- relies on their being a lot of RAM 
- implicit assumption that the queries you are running are on data stored in RAM 
- proprietary system gives you little flexibility; you need to run the data warehouse on top of EXACluster OS (the company's own operating system)

References:
- [1] http://www.exasol.com/en/
- [2] http://en.wikipedia.org/wiki/EXASOL
- [3] http://www.informationweek.com/software/information-management/comparing-vertica-paraccel-and-exasol/d/d-id/1071118?
- [4] http://www.it-director.com/technology/data_mgmt/content.php?cid=10541

**FairCom**  
*C3*  
What:
- database company known for its C-tree technology 

Strengths:
- c-tree Ace (Faircom's product) uses record oriented, indexed sequential access method structure 
- this boosts indexing performance / speed 
- it is a very pluggable system making it a good option for smaller embedded systems with limited resources 
- cross platform and embeddable

Weaknesses:
- not very popular, SQL works for most people
- limited documentation, information available online 

References:
- [1] http://www.faircom.com/ace/products_t.php
- [2] http://dbaspot.com/databases/158221-faircom-c-tree-server-vs-relational-dbms.html
- [3] http://en.wikipedia.org/wiki/C-treeACE


**FatDB**  
*C2*  
What:
- no information found

**67) FathomDB**  
*D5*
What:
- started off as a relational database as a service 
- acquired by Meteor 

Strengths:
- built to handle real time data well 

References:
- [1] http://www.infoq.com/news/2014/10/meteor-fathomdb
- [2] http://www.infoworld.com/article/2676583/database/fathomdb-launches-cloud-database.html


**FeedZai**  
*A2*  
What:
- big data company trying to detect fraud in commerce 
- uses machine learning on top of its massive amount of data 

Strengths:
- handling fraud means insights need to be uncovered quickly, which is why FeedZai is big on realtime processing 

Weaknesses:

References:
- [1] https://www.feedzai.com/home/big-data-insight/
- [2] http://en.wikipedia.org/wiki/Feedzai
- [3] http://www.forbes.com/sites/tomgroenfeldt/2014/02/03/feedzai-brings-machine-learning-and-data-science-to-payment-fraud/

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

**FlockDB**  
*D1*  
What:
- one of the distributed graph databases developed originally by twitter 
- graph database: a database that uses graph structures for queries with nodes, edges, and properties to represent the data 
- sample query you would like a graph database for: What's the intersection of people I follow and people who are following Obama 

Strengths:
- has all the normal stuff like: open source, distributed, fault-tolerant 
- optimized for very large adjacency lists, fast reads and writes 
- much simpler than other graph databases such as Neo4j 

Weaknesses:
- not good for graph traversal operations 
- because FlockDB is built with a rather smaller use case, it doesn't have as many features as some of the other graph databases 

References:
- [1] http://en.wikipedia.org/wiki/FlockDB
- [2] https://blog.twitter.com/2010/introducing-flockdb
- [3] https://github.com/twitter/flockdb
- [4] http://stackoverflow.com/questions/2629692/how-does-flockdb-compare-with-neo4j


**Galera**  
*D4*  
What:
- open sourced database cluster 
- based on synchronous replication
- these things are called high availability solutions 

Strengths:
- there is replication 
- high system uptime
- scales well

Weaknesses:
- cost you money 
- you may not need it over the standard MySQL cluter 


References:
- [1] http://galeracluster.com/
- [2] http://www.quora.com/Who-is-using-MySQL-Galera-in-production
- [3] http://www.percona.com/live/mysql-conference-2012/sessions/how-evaluate-which-mysql-high-availability-solution-best-suits-you



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


**89) Heroku Postgres**
*C5*


**91) HP Autonomy**
*A1*

**92) HP Cloud RDB for MySQL**
*D5*

**93) HP Vertica**
*C6*


**94) HPCC**  
*B6*  

**95) HyperDex**  
*D2*  

**96) HypergraphDB**  
*E1*

**97) Hypertable**  
*C2*  

**98) IBM Big SQL**  
*B4*

**99) IBM BigInsights**  
*A5*

**100) IBM DB2**  
*B4*  

**101) IBM eXtreme Scale**  
*E6*  

**102) IBM IMS**  
*D1*  

**103) IBM InfoSphere**  
*C6*  

**104) IBM PureData**  
*B4*  

**106) InfiniSpan**  
*E6*  

**107) InfiniSQL**  
*C3*  


**108) InfiniteGraph**  
*E1*  


**109) InfluxDB**  
*D6*  

**110) Infobright**  
*B4*  























































