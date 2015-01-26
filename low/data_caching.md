

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