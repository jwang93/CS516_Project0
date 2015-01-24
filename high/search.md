


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




**Azure Search**  
*B2* 
- Microsoft's search as a service platform 
- built on top of Elastisearch, which provides for its text search

Strengths:
- out of the box ease of use; building out a custom search feature for your own company, handling search indices is no trivial task 
- makes scalability very simple especially compared to SOLR which is quite difficult to scale  

Weaknesses:
- expensive 
- commercial and proprietary compared to the open sourced alternative of SOLR  

References: 
- [1] http://azure.microsoft.com/en-us/services/search/
- [2] http://www.tugberkugurlu.com/archive/a-gentle-introduction-to-azure-search
- [3] http://cloudcomputing.sys-con.com/node/3221202
- [4] http://weblogs.asp.net/scottgu/azure-new-documentdb-nosql-service-new-search-service-new-sql-alwayson-vm-template-and-more


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





**Elasticsearch**  
*A1*  
What:
- they have something called an ELK stack of Elasticsearch, Logstash, and Kibana 
- get actionable insight in realtime from structured and unstructured data 
- it's a realtime search and analytics engine 
- can also serve the purpose of a schema-less datastore - something like MongoDB 

Strengths:
- has a RESTful web interface (makes it flexible and usable by many people)
- utilizes schema-free JSON documents 
- open source under an Apache License 
- supposed to have a better distributed model and easier to use than SOLR 

Weaknesses:
- less mature and widely used than Solr, mostly because Solr has been around longer 
- no security whatsoever (authentication or access control)
- no support for transactions or data processing

References:
- [1] http://www.elasticsearch.org/overview/
- [2] http://en.wikipedia.org/wiki/Elasticsearch
- [3] http://stackoverflow.com/questions/10213009/solr-vs-elasticsearch
- [4] http://www.quora.com/Why-should-I-NOT-use-ElasticSearch-as-my-primary-datastore


