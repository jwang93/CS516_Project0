
**Redis**  
*C2*  
What: 
- open sourced key store developed by Pivotal Software and VMWare 
- probably the most popular key store 
- generally holds all data in memory 
- essentially almost always the case that Redis will always be better than memcached 

Strengths:
- some other key stores (such as memcached) only support strings but redis supports abstract data types such as lists, sets, hashes
- super fast at caching - best performance for its use case which is key value data store 

Weaknesses:
- totally in memory so it requires a lot of RAM
- doesn't scale horizontally as well as memcached because redis is more complex 
- can't handle queries as well as something like MongoDB 
- Redis is very good for a specific use case of data retrieval but if you are unclear about your use case it is oftentimes better to go with a more rounded system such as MongoDB 

References:
- [1] http://redis.io/
- [2] http://en.wikipedia.org/wiki/Redis
- [3] http://www.infoworld.com/article/2825890/application-development/why-redis-beats-memcached-for-caching.html
- [4] http://stackoverflow.com/questions/10558465/memcache-vs-redis
- [5] http://stackoverflow.com/questions/5400163/when-to-redis-when-to-mongodb
- [6] http://kkovacs.eu/cassandra-vs-mongodb-vs-couchdb-vs-redis
- [7] http://www.quora.com/What-is-the-difference-between-MongoDB-and-Redis




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




**Ehcache**  
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
