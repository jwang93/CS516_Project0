**Impala**  
*B5*  
What:
- analytic database (also known as query engine) for Hadoop designed by Cloudera 
- often compared against Spark and Hive 
- the advantage of interactive SQL is that you can eliminate the need for temporary data being transferred while you are still querying 

Strengths:
- designed to do massively parallel porcessing (MPP)
- more focused on enterprise customers and use cases 
- Impala, although open source, is still an enterprise product 
- gets good performance for interactive SQL queries on top of Hadoop when compared to Hive - compatible with a lot of other Hadoop software and frameworks such as Hive and Pig 

Weaknesses:
- one of the big drawbacks is that Impala does not allow for in memory processing, which its competitor Spark supports 
- early versions of Impala (and maybe still today) did not support fault tolerance 
- that means that if a node failed in the middle of processing, the entire query would have to be run again 

References:
- [1] http://www.quora.com/Does-Cloudera-Impala-have-any-drawbacks-when-compared-with-Hive
- [2] https://gigaom.com/2014/07/03/cloudera-impalas-it-for-interactive-sql-on-hadoop-but-everything-else-will-move-to-spark/
- [3] http://www.quora.com/How-does-Cloudera-Impala-compare-to-Apache-Shark-now-part-of-Spark
- [4] http://www.cloudera.com/content/cloudera/en/products-and-services/cdh/impala.html
- [5] http://en.wikipedia.org/wiki/Cloudera_Impala
- [6] http://en.wikipedia.org/wiki/Massively_parallel_(computing)
- [7] http://www.quora.com/How-does-Cloudera-Impala-compare-to-Apache-Shark-now-part-of-Spark
- [8] http://www.infoq.com/news/2014/02/SQL-Apache-Hadoop-Impala-Hive



**Google BigQuery**  
*D5*
What:
- service from Google that allows you to interactively query using a SQL-like interface over massive amounts of data 
- you import all your data into Google 
- the service is built on Google's underlying infrastructure 
- marketed as a more powerful, faster alternative to Hadoop although it can be used in conjuction with it 

Strengths:
- easy to access and use this service 
- Google provides a web UI and a RESTful API 
- performance over Hadoop 

Weaknesses:
- costs money 
- not open source, enterprise 

References:
- [1] https://gavinbadcock.wordpress.com/2013/02/06/googles-bigquery-vs-hadoop-complimentors-or-competitors/
- [2] https://cloud.google.com/bigquery/what-is-bigquery
- [3] http://en.wikipedia.org/wiki/BigQuery
- [4] http://news.dice.com/2013/04/15/googles-bigquery-vs-hadoop-a-matchup-2/
- [5] http://www.megapivot.com/blog/posts/redshift-vs-bigquery-vs-hadoop.html




**Apache Drill**   
*B4*  
What:
- open source, SQL query engine for Hadoop and NoSQL
- direct queries on semi-structured data such as JSON with needing to maintain specific schemas 

Strengths:  
- real time data exploration, supposed to be "agile" 
- open source community driven project (can also be a weakness)
- can work on not only Hadoop but also MongoDB, Cassandra, Riak, and Splunk 

Weaknesses:  
- community driven project, makes development a bit more chaotic

References:  
- [1] http://drill.apache.org/
- [2] http://www.quora.com/Isnt-Cloudera-Impala-doing-the-same-job-as-Apache-Drill-incubator-project
- [3] http://gdfm.me/2012/10/27/the-rise-of-the-dremel-clones/
- [4] https://www.mapr.com/products/apache-drill


**Apache Hive**   
** I have experience using Hive before **  
*B4*  

What:
- open source data warehouse software 
- initially came from Facebook 
- DEFN: data warehouse: system used for reporting and data analysis   

Strengths:  
- easy to use due to its abstracted SQL-like language called HiveQL
- has flexibility to plug in custom mappers and reduces 

Weaknesses:  
- basic weakness of batch processing is that it is slow
- imposes the relational rigor of a database (ie schema)

References:  
- [1] https://hive.apache.org/
- [2] http://www.quora.com/What-are-the-pros-and-cons-between-Pig-and-Hive
- [3] http://stackoverflow.com/questions/9569009/what-are-the-pros-and-cons-of-running-a-job-in-hadoop-using-various-languages




**Apache Tajo**   
*B3*  
What:
- relational, distributed data warehouse system built on Hadoop 
- SQL query processing engine 
- one of the growing number of SQL-on-Hadoop frameworks 

Strengths:  
- can adjust query processing based on: user queries, characteristics of data, cluster status
- supports SQL standards which gives it a lower barrier to entry 
- great performance (way better than Hive) and better than Impala on: filters, group by, join, filter scan 

Weaknesses:  
- worse than Impala when you do a union and then join
- smaller community as it is developed in Korea may not make it worth it when you have really good alternatives in Impala and Presto 

References:  
- [1] http://mail-archives.apache.org/mod_mbox/tajo-dev/201305.mbox/%3CCACZfFK6PNE+AuNX6CQ0WD784ZxUavEykEKa-rWFMXp0xdyAHmg@mail.gmail.com%3E
- [2] http://tajo.apache.org/
- [3] http://blogs.gartner.com/nick-heudecker/apache-tajo-enters-the-sql-on-hadoop-space/
- [4] http://blog.matthewrathbone.com/2014/06/08/sql-engines-for-hadoop.html#apache-tajotajo



**AWS Redshift**   
*D6*  
What:
- data warehouse solution that makes it easy to do analysis on the data using your own business analytics tools

Strengths:  
- fast query performance from columnar storage 
- offers a wide range of SQL clients: PostgreSQL
- also it's pretty cheap compared to its competitors (unusual for AWS) 

Weaknesses:  
- doesn't have uniqueness so you need to make sure you haven't already written your data to Redshift 
- quite difficult to do ETL 
- doesn't have the features that a competing product like Hive has 

References:  
- [1] http://aws.amazon.com/redshift/
- [2] http://www.quora.com/What-are-some-good-real-world-examples-of-using-Amazon-redshift
- [3] http://www.quora.com/What-are-the-pros-and-cons-of-using-Amazon-Redshift





**Couchbase**  
*C2*  
What:
- NoSQL document oriented database great for applications that are interactive 

Strengths:
- handle many concurrent users 
- scales up with low latency and high throughput 
- based on memcache which is proven to be super fast (hard to get better performance than Couchbase)

Weaknesses:
- fewer querying and indexing options compared to competitor MongoDB 
- doesn't have good dynamic query support compared to Mongo

References:
- [1] http://www.couchbase.com/nosql-resources/what-is-no-sql
- [2] http://en.wikipedia.org/wiki/Couchbase_Server
- [3] http://www.infoworld.com/article/2613970/nosql/nosql-showdown--mongodb-vs--couchbase.html
- [4] http://www.quora.com/How-does-Riak-compare-to-Couchbase



