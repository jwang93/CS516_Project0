


**Apache S4**  
*A2*  
What:
- made more for processing continuous streams of data (real time data ingestion)
- can be compared to Twitter Storm 

Strengths:  
- good for stream/real-time applications (don't want to do batch)
- data is optimized for a stream 
- modular and pluggable: many of the components can be replaced on developer discretion

Weaknesses:  
- data reliability 
- apparently it's quite buggy? 

References:  
- [1] http://incubator.apache.org/s4/ 
- [2] http://www.quora.com/How-does-S4-compare-to-Flume
- [3] http://www.quora.com/What-would-you-choose-between-Flume-Yahoo-S4-and-Backtype-Twitter-Storm-and-why



**Apache Storm**   
*A2*   
What:
- distributed realtime computation system initially developed out of Twitter
- trying to do for realtime processing what Hadoop did for batch 
- operates on data in motion, not data at rest 

Strengths:  
- the spout abstraction makes it easy to integrate with a number of queuing and database systems 
- great for low latency results and no data loss 
- widely used with a large and active community 

Weaknesses:  
- narrow in that it only allows for one type of input - the stream 
- doesn't support exactly-once processing, may perform duplicate processing called "at least once processing"

References:  
- [1] https://storm.apache.org/ 
- [2] http://www.quora.com/What-is-the-difference-between-Apache-Storm-and-Apache-Spark
- [3] http://xinhstechblog.blogspot.co.uk/2014/06/storm-vs-spark-streaming-side-by-side.html
- [4] http://stackoverflow.com/questions/15520993/storm-vs-trident-when-not-to-use-trident


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



**AWS EMR**   
*A4*  
What:
- stands for Elastic Mapreduce 
- uses Hadoop to do the data distribution and computation but can also use Spark or Presto

Strengths:  
- the ability to get computation on tap 
- lots of the details are managed for you 
- lowest barrier to usage 

Weaknesses:  
- keeping it running is expensive 
- doesn't have features like automatic cluster lifecycle management, automatically scaling up and down
- known to get unstable at scale 

References: 
- [1] http://aws.amazon.com/elasticmapreduce/
- [2] http://www.quora.com/What-is-your-feedback-of-using-Amazons-EMR-or-Hadoop-on-EC2-or-CDH-for-Telecoms-data-CDR-Recharge-Transactions-others-event-data
- [3] http://engineering.pinterest.com/post/92742371919/powering-big-data-at-pinterest


