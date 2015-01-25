**ClearDB**  
*D5*  
What:
- database for MySQL applications 
- impressive customer set of Microsoft and salesforce 

Strengths:
- fault tolerant, which means that if a component fails, a backup system can come back up immediately with no need for human maintenance 
- can support database size up to 10GB 

Weaknesses:
- doesn't have the community of Amazon RDS 
- easy to set up (< 1 minute) but you need to use one of their partners: Heroku, Appfog, Azure cloud 

References:
- [1] https://www.cleardb.com/
- [2] http://w3facility.org/question/xeround-vs-cleardb-hosted-mysql-pros-and-cons/
- [3] http://www.sitepoint.com/database-as-a-service-mysql-in-the-cloud/



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




**DeepDB**  
*D4*  
What:
- branded as a general purpose database for big data 

Strengths:
- built to provide good performance while scaling up 
- done through writing indexes quickly 
- good for OLTP 
- can perform realtime ACID transactions (similar to that of a normal relational database) and analytics on the same data set 

Weaknesses:
- tough to sell a new type of databae to enterprise customers who prefer to continue using what they have 
- "keep on using something until it breaks"
- introduces a new product in an already very mature and congested space 
- limited community, not much readily available information on it

References:
- [1] http://deep.is/deepdb/
- [2] http://www.dbms2.com/2013/04/14/deep-information-sciences-deepdb/
- [3] http://www.severalnines.com/news/article/database-clustering/is-deepdb-a-good-general-purpose-choice-for-big-data-needs/801612841



**Drizzle**  
*C4*  
What:
- open source cloud RDBMS forked off MySQL 
- moved all the non essential components of MySQL out into modules that can be added independently 

Strengths:
- supposed to be a trimmed down version of MySQL
- this should give it a performance boost 
- cache and optimization components more pluggable than MySQL 
- supposed to be designed for web applications and cloud computing 
- free

Weaknesses:
- project is kind of dead right now, last stable release was 2 years ago
- not well supported
- competitor MySQL works fine for most use cases 

References:
- [1] http://www.drizzle.org/
- [2] http://en.wikipedia.org/wiki/Drizzle_(database_server)
- [3] http://db-engines.com/en/system/Drizzle%3BMySQL
- [4] http://www.linuxuser.co.uk/news/mysql-successor-drizzle-reaches-maturity
- [5] http://www.quora.com/Why-is-Drizzle-dead



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



