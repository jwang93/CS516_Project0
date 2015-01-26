
**AWS RDS**   
*D5*  
What:
- Amazon's version of a traditional relational database in the cloud 
- you can compare it to a self hosted MySQL 

Strengths:  
- comes with all the Amazon managed goodies (backups, patch management, and replication)
- have this feature called multi AZ which stands for multi availability, which handles replication and backups for failure 
- it also gives a very good up time ~99.95% 

Weaknesses:  
- couple drawbacks to RDS when you are doing complex operations that require many privileges 
- doesn't have very high security needs 
 
References:  
- [1] http://aws.amazon.com/rds/
- [2] http://www.laurencegellert.com/2013/05/pros-and-cons-of-rds-vs-ec2-for-mysql-with-aws/
- [3] https://www.scalebase.com/aws-rds-vs-self-hosted-mysql-availability-scalability-performance/

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




