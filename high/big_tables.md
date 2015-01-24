
**HBase**  
*C2*  
What:
- open source, non-relational distributed database that was modeled after Google's BigTable 
- runs of top of HDFS meaning that it interfaces well with Hadoop 
- DEFN: Bloom Filter: probabilistic data structure that can determine whether an element exists in a set 
- HBase is column oriented and well suited for sparse data sets 
- from an architecture standpoint, HBase is more centralized with a master that watches over a bunch of worker nodes; Cassandra is more decentralized where any node can do any operation 

Strengths:
- good for storing large quantities of sparse data 
- an example would be you have billions of records, but only care about the top 5 or so 
- has a feature for Bloom filters, which is what Professor Babu mentioned in class 
- has a native Java API, using Java is a huge plus for some because there are a ton of libraries in Java

Weaknesses:
- doesn't have support for SQL, which is the de facto standard 
- its similar counterpart - Cassandra - does have support for something called CQL (cassandra query language) which is modeled after SQL
- if you must continue using SQL, this weakness ofr HBase may push the direction in favor of Cassandra
- like Cassandra, there is no real support for transactions 
- much weaker documentation compared to Cassandra 

References:
- [1] http://hbase.apache.org/
- [2] http://en.wikipedia.org/wiki/Apache_HBase
- [3] http://en.wikipedia.org/wiki/Bloom_filter
- [4] http://www-01.ibm.com/software/data/infosphere/hadoop/hbase/
- [5] http://www.infoworld.com/article/2610656/database/big-data-showdown--cassandra-vs--hbase.html?page=3
- [6] http://bigdatanoob.blogspot.com/2012/11/hbase-vs-cassandra.html
- [7] http://www.quora.com/What-are-the-differences-between-HBase-and-Cassendra



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


