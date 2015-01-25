

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



**CodeFutures**  
*C4*  
What:
- big data company that has a suite of products
- focus is on database sharding, product called dBshards 
- have another product called Firestorm which is used for DAO (database access object) 

Strengths:
- providing the benefits of sharding (splitting data across multiple data centers) with little effort
- CodeFutures empowers traditional MySQL databases to do Big Data by allowing to shard the data 

Weaknesses:
- data is partitioned not at the application level (some such as Adam D'Angelo view as bad) 

References: 
- [1] http://en.wikipedia.org/wiki/CodeFutures
- [2] http://codefutures.com/codefutures-blog/
- [3] http://www.quora.com/How-can-MySQL-be-used-for-big-data-analysis
- [4] http://www.quora.com/What-kind-of-layer-should-there-be-between-the-application-level-and-the-database-level-in-order-to-scale-out



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



**Galera**  
*D4*  
What:
- open sourced database cluster 
- based on synchronous replication
- these things are called high availability solutions 

Strengths:
- there is replication 
- high system uptime
- scales well

Weaknesses:
- cost you money 
- you may not need it over the standard MySQL cluter 


References:
- [1] http://galeracluster.com/
- [2] http://www.quora.com/Who-is-using-MySQL-Galera-in-production
- [3] http://www.percona.com/live/mysql-conference-2012/sessions/how-evaluate-which-mysql-high-availability-solution-best-suits-you



