
**CitusDB**  
*B5*  
What:
- database system focused on scaling out PostgreSQL
- done via sharding and replication 

Strengths:
- supports semi structured data over JSON and log files 
- strong performance numbers, seems to perform slightly better than Impala in some benchmarks
- PostgreSQL at the core which is an incredibly popular open sourced database with many features

Weaknesses: 
- read a blog that stated that CitusDB was really fast for some basic benchmarks 
- however when he wanted to run complex queries - utilizing distinct and subqueries - CitusDB didn't work and he had to change to Redshift 

References:
- [1] http://haifzhan.blogspot.com/2014/03/citusdb-experience.html
- [2] http://www.quora.com/How-does-CitusDB-compare-to-Cloudera-Impala
- [3] http://www.citusdata.com/blog/86-making-postgresql-scale-hadoop-style


