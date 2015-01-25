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



