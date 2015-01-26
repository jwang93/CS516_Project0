
**Riak**  
*C2*  
What:
- open source distributed database developed by Basho
- also has the functionality of a NoSQL system, key value data store 
- compared to Cassandra, both of which are based off of Amazon's Dynamo  

Strengths:
- Basho cites the strengths of Riak being 
- low latency: getting great performance even under heavy load
- scalable and available
- has a built in REST server making it easy to set up and use, operationally simple to maintain
- one of the problems with Mongo is the working set needs to fit in memory, which is not a requirement for Riak

Weaknesses:
- if you want to do multi data center replication, you need to purchase the enterprise product 
- can't perform the range query as fast as Cassandra due to the differences in architecture between the two 

References:
- [1] http://basho.com/riak/
- [2] http://en.wikipedia.org/wiki/Riak
- [3] https://blog.mozilla.org/data/2010/05/18/riak-and-cassandra-and-hbase-oh-my/
- [4] http://nosql.mypopescu.com/post/30830925905/from-mongodb-to-riak-at-shareaholic
- [5] http://basho.com/riak-vs-cassandra/



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




**Cassandra**  
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




**FoundationDB**  
*C2*  
What:
- multi model NoSQL database 
- what does multi model mean?
- database that can support multiple models, where a model can be document, graph, relational, key value 

Strengths:
- can support multiple models in the same database, specifically key value, SQL, document, and graph

Weaknesses:
- doesn't have support for long transactions - specifically transactions over 5 seconds 
- doesn't have support for large transactions - ones that exceed 10MB 
- doesn't have support for large keys or values - keys can't be over 10KB and values can't be over 100KB 
- essentially, because FoundationDB is so flexible with its multi-model database, the tradeoff is that you get a number of limitations
- ultimately, you need to ask yourself how much value add the multi model support is 

References:
- [1] https://foundationdb.com/key-value-store/documentation/known-limitations.html
- [2] http://en.wikipedia.org/wiki/FoundationDB
- [3] http://en.wikipedia.org/wiki/Multi-model_database
- [4] http://blog.foundationdb.com/call-me-maybe-foundationdb-vs-jepsen
- [5] http://opensourceconnections.com/blog/2013/03/06/why-foundationdb-might-be-all-its-cracked-up-to-be/



