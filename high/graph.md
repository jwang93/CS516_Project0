**Allegrograph**  
*E1*  
What:
- specifically a graph database 
- uses combination of memory and disk allowing for huge scale 
- utilizes an RDF store (triple store of the form - subject:predicate:object)

Strengths:  
- huge scale due to its usage of disk 
- has a java client library that supporst Jena and Sesame 
- supports SPARQL queries 

Weaknesses:  
- there are competing graph databases that are open source, Allegro is commercial license
- not embeddable compared to competitor Neo4J 
- doesn't support MapReduce? 

References:  
- [1] http://franz.com/agraph/allegrograph/
- [2] http://db-engines.com/en/system/AllegroGraph%3BNeo4j%3BVoltDB
- [3] http://stackoverflow.com/questions/2613357/difference-between-graph-database-neo4j-allegrograph
- [4] http://vschart.com/compare/allegrograph/vs/neo4j




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



**FlockDB**  
*D1*  
What:
- one of the distributed graph databases developed originally by twitter 
- graph database: a database that uses graph structures for queries with nodes, edges, and properties to represent the data 
- sample query you would like a graph database for: What's the intersection of people I follow and people who are following Obama 

Strengths:
- has all the normal stuff like: open source, distributed, fault-tolerant 
- optimized for very large adjacency lists, fast reads and writes 
- much simpler than other graph databases such as Neo4j 

Weaknesses:
- not good for graph traversal operations 
- because FlockDB is built with a rather smaller use case, it doesn't have as many features as some of the other graph databases 

References:
- [1] http://en.wikipedia.org/wiki/FlockDB
- [2] https://blog.twitter.com/2010/introducing-flockdb
- [3] https://github.com/twitter/flockdb
- [4] http://stackoverflow.com/questions/2629692/how-does-flockdb-compare-with-neo4j



