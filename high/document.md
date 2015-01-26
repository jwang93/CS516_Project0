
**MongoDB**   
*E2*   
What:
- one of the most popular NoSQL databases, it is document oriented 
- shuns the traditional relational database schema for JSON like objects 

Strengths:
- supports full indexing - primary and secondary
- huge community of users; tested and ready for production environments
- it is open source and free to use 
- it has a flexible schema - you could even all it schema-less 
- this is a huge value if you are still in the early stages of your use case and you aren't sure how your data is going to be laid out 
- performs better if your application is more read intensive than write 
- there is built in sharding in MongoDB which doesn't exist for MySQL 

Weaknesses:
- by virtue of being document oriented, you lose some functionality that traditional RDBMS has, specifically JOINs 
- there is no current support for transactions 
- not as mature as the traditional RDBMS 
- development is very fast so the system is changing pretty rapidly 

References:
- [1] http://www.mongodb.org/
- [2] http://en.wikipedia.org/wiki/MongoDB
- [3] http://www.sarahmei.com/blog/2013/11/11/why-you-should-never-use-mongodb/
- [4] http://stackoverflow.com/questions/5244437/pros-and-cons-of-mongodb
- [5] http://www.quora.com/What-are-the-pros-and-cons-of-Mongo-DB-compared-to-MySQL-database
- [6] http://www.quora.com/Document-oriented-Databases/Can-someone-weigh-the-pros-and-cons-of-MongoDB-vs-Clusterpoint-software-I-cant-find-much-on-Clusterpoint-as-they-havent-really-penetrated-markets-outside-of-Latvia-yet



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




**MemSQL**  
*C3*  
What:
- in memory database
- member of the NewSQL database systems
- lot of hype around MemSQL: self proclaimed to be fastest in the world due to being distributed in memory and using a column store engine 
- by having all the data in memory, MemSQL handles persistance by keeping transaction logs and writing out the data every so often 

Strengths:
- very high performance 
- it can ingest and process data quickly 
- will beat a traditional PostgreSQL operation because it keeps all the data in memory and it converts the SQL code into C++ (which is fast)

Weaknesses:
- can't scale beyond a single node
- need lots of memory to support this system's speed 

References:
- [1] http://www.memsql.com/
- [2] http://en.wikipedia.org/wiki/MemSQL
- [3] http://www.quora.com/What-are-the-advantages-of-MemSQL-over-PostgreSQL-in-which-specific-cases-would-the-former-be-better-than-the-latter
- [4] http://www.quora.com/SQL/What-benefits-does-MemSQL-offer-over-running-a-MySQL-database-on-ramdisk




**IBM DB2**  
*C4*  
What:
- family of database servers released by IBM dating back to the 1980s 
- traditionally have supported the relational model
- however, in recent years to meet the new demand, they have experimented with document oriented models are well 

Strengths:
- DB2 is more of an enterprise product although there are many enterprises that use open sourced products like MySQL
- being enterprise and more mature comes with a standard suite of features like disaster recovery, high availability, scaling 
- can store XML natively and retrieve them using xPath, xQuery 

Weaknesses:
- if you are looking for something simpler there are better options such as MySQL
- like every enterprise product, will cost you money, which is unattractive especially when there are free alternatives 

References:
- [1] http://www-01.ibm.com/software/data/db2/
- [2] http://en.wikipedia.org/wiki/IBM_DB2
- [3] http://www.ehow.com/info_12106599_advantages-db2.html
- [4] http://db-engines.com/en/system/DB2%3BMySQL
- [5] http://stackoverflow.com/questions/9299127/mysql-vs-db2-rdbms





**MongoLab**  
*E2*    
What:
- cloud database service that will host MongoDB databases 
- you can think of it as a MongoDb as a service 

Strengths:
- ease of use 
- have a free plan which is good for startups, school projects
- would be great to use for our CS516 final project if we were using MongoDB
- great customer support 

Weaknesses:
- won't be able to support heavy customization 

References:
- [1] https://mongolab.com/
- [2] http://en.wikipedia.org/wiki/MongoLab
- [3] http://mrdanadams.com/2012/mongohq-mongolab-mongodb-customer-service/#.VMV6Xy6Ynxg
- [4] http://webmasters.stackexchange.com/questions/20782/mongodb-hosting-mongolab-vs-mongohq-vs-mongomachine
- [5] http://www.quora.com/What-is-the-best-mongodb-hosting


**Azure DocumentDB**  
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



**CouchDB**  
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


