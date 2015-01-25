
**Accumulo**    
*D2*  
What:  
- sorted, distributed key-value store 
- based on Google BigTable 
- built on Hadoop, Zookeeper, and Thrift   

Strengths:  
- high availability 
- sorted and distributed 
- scales well while delivering good performance  

Weaknesses: 
- does not support a "NOT" operator.. for security reasons
- when compared to HBase, Accumulo is less popular and thus has fewer integrations with other systems

References: 
- [1] https://accumulo.apache.org/ 
- [2] http://www.cloudera.com/content/cloudera/en/products-and-services/cdh/accumulo.html
- [3] http://apache-accumulo.1065345.n5.nabble.com/How-does-Accumulo-compare-to-HBase-td10464.html  



**Cassandra.io**  
*D2*  
What:
- a hosted and managed instance of Cassandra that is made accessible via a RESTful API 

Strengths:
- makes Cassandra even easier to use, especially for any kind of web programming that could utilize an API 
- on the data platforms chart, Cassandra.io sits on the "as a service" category which makes sense 

Weaknesses:
- the additional level of abstraction doesn't give developers as much flexibility as if they used a manually configured standalone Cassandra instance 

References:
- [1] https://bighadoop.wordpress.com/2012/09/09/heroku-and-cassandra-cassandra-io-restful-apis/



**DataStax Enterprise**  
*C2*  
What:
- platform built on Apache Cassandra for analytics for online database applications 

Strengths:
- DataStax basically provides Apache Cassandra but with a bunch of tools and features on top on Apache Cassandra
- easy to set up and maintain 

Weaknesses:
- costs money whereas vanilla Cassandra is free 

References:
- [1] http://www.datastax.com/what-we-offer/products-services/datastax-enterprise
- [2] http://stackoverflow.com/questions/24564725/apache-cassandra-vs-datastax-cassandra

