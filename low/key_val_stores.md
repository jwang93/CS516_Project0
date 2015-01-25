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


