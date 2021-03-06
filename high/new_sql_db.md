
**Hortonworks**  
*A5*  
What:
- a company that builds a variety of solutions for Hadoop 
- they are main competitors with Cloudera and MapR; the emergence of these enterprise Big Data companies 
- they perform a lot of open source development for Hadoop 
- all of these Hadoop distribution providers make their money by selling a suite of services on top of their software 

Strengths:
- Hortonworks and Cloudera provide nearly 100% open source distributions of Hadoop, something their competitor MapR does not do (they have more proprietary modules)
- these are the guys who came out with YARN which is a new version of Hadoop better than the previous MapReduce; YARN allows the inclusion of more data processing frameworks 

Weaknesses:
- because Hortonworks' distribution is completely open source, it is not as enterprise ready as something like MapR's distribution 
- they don't have the reach of Cloudera, who has been around the longest and has the most number of customers
- this does give Cloudera a bit of an edge in terms of knowing what features are needed 

References:
- [1] http://hortonworks.com/hadoop-modern-data-architecture/
- [2] http://en.wikipedia.org/wiki/Hortonworks
- [3] http://www.experfy.com/blog/cloudera-vs-hortonworks-comparing-hadoop-distributions/
- [4] http://www.quora.com/What-are-some-major-pros-cons-of-Cloudera-vs-Hortonworks-as-a-Hadoop-platform-for-a-main-street-e-g-not-Silicon-Valley-giant-enterprise
- [5] http://www.quora.com/What-distribution-should-I-choose-Cloudera-Hortonworks-or-MapR

**GenieDB**  
*C4*  
What:
- globally distributed MySQL as a service 
- built a replication system that is very automated 

Strengths:
- focused on having high availability
- naturally, as an as-a-service platform it's quite easy to use 
- reliable 

Weaknesses:
- costs money 
- not widely used, not much documentation 

References:
- [1] https://aws.amazon.com/marketplace/pp/B00C1OVTMQ/ref=tsm_geniedb
- [2] http://www.zdnet.com/article/geniedb-global-distributed-database-as-a-service/



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


