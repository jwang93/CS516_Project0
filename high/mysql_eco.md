
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




