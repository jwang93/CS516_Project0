
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


