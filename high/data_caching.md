
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
