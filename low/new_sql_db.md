
**Altibase HDB**   
*D3*  
What:
- hybrid in memory database, hence the name HDB developed by altibase 
- utilizes spatial indexing 

Strengths:  
- purported to be very fast (although this is from Altibase)
- lot of features that competitors don't have such as - SQL Interpreter, Java Support, Real Time Access

Weaknesses:  

References:  
- [1] http://altibase.com/in-memory-database-hybrid-products/hdbtm-hybrid-dbms/
- [2] http://database-management.findthebest-sw.com/compare/5-36/ALTIBASE-HDB-vs-Oracle 



**Altibase XDB**   
*D3*  
What:
- XDB stands for extreme in memory database - memory only 
Strengths:  
- very fast 

Weaknesses:  
- requires a lot of memory 
- can't utilize disk 
- limited operating systems support 

References:  
- [1] http://altibase.com/in-memory-database-hybrid-products/xdb/




**Clusrix**  
*C4*  
What:
- ecommerce databaes good for online retailers
- calling itself a "NewSQL database"
- RDBMS systems that are trying to provide the scale of these NoSQL systems while still guaranteeing the great properties of RDBMS like ACID 
- relational database that can scale horizontally as you add more servers 

Strengths:
- scaling transactions, don't want customers to worry about whether their relational database can keep up 
- real time analytics 
- ACID 
- easy to migrate from MySQL to Clustrix 

Weaknesses:
- cost 

References:
- [1] http://www.clustrix.com/
- [2] http://en.wikipedia.org/wiki/Clustrix
- [3] http://blog.clustrix.com/2012/12/11/what-does-it-mean-to-say-clustrix-is-a-mysql-replacement/



**CockroachDB**  
*C3*  
What:
- transactional geo-replicated data store 
- DEFN: geo-replication is when you keep multiple copies of the data in various geographical locations to speed up the response times of queries 

Strengths:
- very resilient (why it's called CockroachDB), supposed to never fail 
- if one server goes down, another one will be available 
- built for scalability, transactionability, availability 

Weaknesses:
- with all this focus on availability and resiliency, there is probably a performance hit 

References:
- [1] http://cockroachdb.org/
- [2] https://news.ycombinator.com/item?id=7823076
- [3] http://www.quora.com/What-are-some-good-uses-for-CockroachDB-the-open-source-implementation-of-Google-Spanner
- [4] http://www.wired.com/2014/07/cockroachdb/



**Continuent**  
*D4*  
What:
- provide services for database clustering and replication
- DEFN: clustering is when you have several servers connect to a single database
- allows for fault tolerance if one server were to fail
- load balancing, sending the user to the server with lowest load 

Strengths:
- managed for you 
- replication and recovery 
- allows for fault tolerance if one server were to fail
- load balancing, sending the user to the server with lowest load 

Weaknesses:
- pretty lackluster community
- couldn't find much research on it 

References:
- [1] http://www.continuent.com/solutions
- [2] http://www.techopedia.com/definition/17/clustering-databases
- [3] http://www.quora.com/Is-MySQL-Proxy-ready-for-production-use



**Datomic**  
*C3*  
What:
- transactional, cloud-ready, distributed database 
- implement Datalog 

Strengths:
- kind of like a hybrid between NoSQL and SQL systems
- so you get a minimal schema while still allowing for Joins 
- comes with enterprise support 

Weaknesses:
- doesn't provide all the benefits of a NoSQL system like the schema-less document object storage model of MongoDB

References:
- [1] http://www.datomic.com/rationale.html
- [2] http://en.wikipedia.org/wiki/Datomic
- [3] http://comments.gmane.org/gmane.comp.db.datomic.user/9



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


