
**Altiscale**  
** I have used Altiscale before at my previous internship at Drawbrdge **  
*A3*  
What:
- company that provides Hadoop cloud services, they run your Hadoop workloads for you 
- notion of Hadoop as a Service 

Strengths:  
- easy to use, configurations all handled for you, customer support 
- cloud nature can handle variability of Hadoop workloads 
 
Weaknesses:  
- expensive - would be much cheaper to roll out your own Hadoop infrastructure 
- less control over your Hadoop jobs than if you ran it yourself 

References:  
- [1] https://www.altiscale.com/why-altiscale/




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



**Cloudera**  
*A5*  
What:
- multi billion dollar company that provides Hadoop based software and services
- products include: CDH (cloudera distributed hadoop), Spark , Impala, Search

Strengths:
- rather than wade through the many versions of Hadoop and tools associated with it, CDH is a neatly packaged and documented bundle of all Hadoop + Hadoop related tools to make for a more enjoyable development experience 
- some of Cloudera's solutions have been around longer and are more mature than its competitor's solution Hortonworks 

Weaknesses:
- Cloudera's services are expensive (you can download CDH for free but it won't have any technical support or Cloudera manager)
- selling commerical software on top of its open sourced distribution 

References:
- [1] http://www.cloudera.com/content/cloudera/en/products-and-services/cdh.html
- [2] http://en.wikipedia.org/wiki/Cloudera
- [3] http://www.quora.com/Can-someone-provide-comparative-analysis-of-Cloudera-and-Hortonworks
- [4] http://www.b-eye-network.com/blogs/eckerson/archives/2014/02/the_battle_for.php



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



**Databricks/Spark**  
*A5*  
What:
- open source processing engine for Hadoop data 
- Spark is now an Apache project but Databricks is a main developer for it

Strengths:
- speed (up to 100x faster in memory, 10x on disk)
- flexibility in that it can use either memory or disk unlike Hadoop which uses HDFS (disk)
- enormous open source community 
- features beyond basic map and reduce: allows for SQL queries, streaming data, machine learning libraries 
- great for iterative processing, interactive processing, and event stream processing ]

Weaknesses:
- pretty young system so still some bugs, not nearly as mature as Hadoop 

References:
- [1] https://databricks.com/spark
- [2] http://en.wikipedia.org/wiki/Apache_Spark
- [3] http://www.quora.com/What-are-the-pros-and-cons-of-Apache-Spark
- [4] http://www.javaworld.com/article/2360185/big-data/straight-talk-on-apache-spark-and-why-you-should-care.html
- [5] http://stackoverflow.com/questions/25267204/hadoop-vs-spark



