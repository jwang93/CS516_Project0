
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



