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


**Neo4J**  
*C1*  
What:
- open sourced graph database
- often compared to Titan
- data is stored as either an edge, node, or attribute 
- edges and nodes can have multiple attributes 

Strengths:
- data is stored on disk, not a significant memory requirement 
- very fast because the storage of data is on the same machine as where the query engine is on
- that does lead to limitations such as inability to scale horizontally	
- as with any graph database, it is really good at looking up relationships between nodes 
- so if you are trying to solve any kind of graph problem: Pinterest, Facebook, Linkedin

Weaknesses:
- cannot be sharded which means that all the data needs to be kept in one server 
- one of the competitors - Titan - can scale horizontally
- scaling horizontally vs scaling vertically
- scaling horizontally (preferred) is simply adding more servers
- scaling vertically (what Neo4j does) is adding more resources to a server 

References:
- [1] http://neo4j.com/
- [2] http://en.wikipedia.org/wiki/Neo4j
- [3] http://www.slideshare.net/seenickcode/migrating-from-mongodb-to-neo4j-lessons-learned
- [4] https://groups.google.com/forum/#!topic/neo4j/mts6H9Py-2I
- [5] http://www.quora.com/What-are-the-pros-and-cons-of-using-a-graph-database
- [6] http://stackoverflow.com/questions/17269306/anybody-tried-neo4j-vs-titan-pros-and-cons
- [7] https://groups.google.com/forum/#!msg/aureliusgraphs/vkQkzjN8fo0/9YYgqI4TA0QJ
- [8] http://stackoverflow.com/questions/5401992/what-does-scale-horizontally-and-scale-vertically-mean




**MySQL**  
*C4*  
What:
- one of the most popular open source RDBMS currently developed by Oracle
- it is used heavily for web development as it is a critical component of the LAMP stack

Strengths:
- learning curve is pretty low compared to Postgres
- getting Postgres configured, creating a user, etc, was a bit of pain
- free to use 
- can run on Linux, which is a draw because that is the operating system of choice for many web servers 

Weaknesses:
- not as mature as other open sourced databases such as PostgreSQL
- development is not community driven but rather driven by Oracle 
- this can actually be a strength though, it depends on whether you value a slower more robust enterprise development
- from a performance standpoint, I've seen people citing that Postgres benchmarks a little better than MySQL but the difference is marginal 

References:
- [1] http://www.mysql.com/
- [2] http://en.wikipedia.org/wiki/MySQL
- [3] http://www.smartfile.com/blog/the-pros-and-cons-of-mysql/
- [4] https://www.digitalocean.com/community/tutorials/sqlite-vs-mysql-vs-postgresql-a-comparison-of-relational-database-management-systems
- [5] http://stackoverflow.com/questions/4779029/why-is-mysql-used-so-often-in-web-development
- [6] http://www.sitepoint.com/forums/showthread.php?34311-Why-is-MySQL-so-popular
- [7] http://www.quora.com/Why-is-MySQL-more-popular-than-PostgreSQL
- [8] http://www.wikivs.com/wiki/MySQL_vs_PostgreSQL




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



