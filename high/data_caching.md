
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



**Voldemort**  
*C2*   
What:
- distributed, fault tolerant data store built by Linkedin that operates as a normal key-value data store
- you can liken it to a large distributed hash table 

Strengths:
- combination of in memory caching with storage system making the storage system fast
- scales horizontally well for reads and writes 
- very fast - over 10,000 operations per second, although other competitors such as Cassandra can also deliver this performance 
- couple sources have cited its super simple and easy to use API 

Weaknesses:
- functionality is limited to that of just key-value store whereas Cassandra offers more features such as range queries 
- isn't much structure to the data; Cassandra provides something called column families which give the data more sturcture 
- not as popular as Cassandra and thus not as well supported

References:
- [1] http://en.wikipedia.org/wiki/Voldemort_(distributed_data_store)
- [2] http://www.project-voldemort.com/voldemort/
- [3] http://stackoverflow.com/questions/2252163/how-does-voldemort-compare-to-cassandra
- [4] http://stackoverflow.com/questions/17341527/nosql-db-hbase-vs-voldemort-vs-couchbase
- [5] http://blog.medallia.com/product-and-innovation/choosing-a-key-value-storage-system-cassandra-vs-voldemort/



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




**Couchbase**  
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
