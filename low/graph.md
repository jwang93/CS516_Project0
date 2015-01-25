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


**AffinityDB**   
*E1*  
What: 
- platform for information processing, control
- at its core it is a graph database
- runs something called pathSQL 

Strengths:  

Weaknesses:  
- little information / documentation on affinityDB

References:
- [1] http://affinityng.cfapps.io/doc/terminology.html#pathsql


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



