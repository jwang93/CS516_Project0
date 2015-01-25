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





