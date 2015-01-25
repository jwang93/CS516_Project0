**1010data**  
*D6*  
What:  
- database with spreadsheet interface
- customers like Clorox, Morgan Stanley
- B2B enterprise company
- replacement to traditional data warehouse  

Strengths:  
- easy to use, don't need deep technical knowledge 
- cloud based so can be accessed anywhere 
- provides clients with industry specific solutions
- NoSQL

Weaknesses:  
- technical portion is heavily abstracted 
- limitations to what a client can do 

References:   
- [1] https://www.1010data.com/products/detail/1010data-industry-specific-applications
- [2] http://www.itworld.com/article/2730562/big-data/1010data--the-non-elephant-in-the-big-data-room.html 




**Actian Matrix**  
*C6*  
What:  
- analytics database from Actian

Strengths:  
- comes with many built in algorithms courtesy of Actian
- parallel, columnar, compressed
- compiles queries during query execution which reduces overhead 
- has an option to be run entirely in memory 

Weaknesses:  
- expensive

References:  
- [1] http://wwwcdn.actian.com/wp-content/uploads/2014/01/Actian-Matrix-Datasheet.pdf



**Actian Vector**  
*C6*  
What:  
- analytical database system 
- successor to MonetDB
- SQL on Hadoop 

Strengths:  
- data partitioning and parallel load feature allow for shorter data loading time 
- performance boosts from compression and better I/O scheduling 

Weaknesses:  
- doesn't really scale out that well 
- expensive 

References:  
- [1] http://www.actian.com/about-us/blog/vectorwise-goes-hadoop/ 
- [2] http://www.actian.com/about-us/blog/pssst-want-hear-actian-vector-3-5/ 
- [3] http://www.dbms2.com/2013/04/25/goodbye-vectorwise-farewell-paraccel/



**ArangoDB**   
*B2*  
What: 
- open source, NoSQL database 
- multi model database 

Strengths:  
- great for documents, graphs, and key values
- supports a SQL like query language making it easy to use
- supports some JavaScript extensions 
- multi model database allows for different data models (graphs and documents) in the same application that might even need to be mixed in the same query 

Weaknesses:  
- not embeddable like its competitor OrientDB 
- the restriction on the max value size is 256MB compared to 2GB for a competitor 

References:  
- [1] https://www.arangodb.com/
- [2] http://vschart.com/compare/arangodb/vs/orientdb
- [3] http://stackoverflow.com/questions/26704134/mongodb-neo4j-vs-orientdb-vs-arangodb



**BitYota**  
*D6*  
What:
- tagline of "Data Warehouse as a service"
- ingest data from a number of sources and perform analysis 

Strengths:
- easy to set up and maintain as it is managed for you 
- supports standard ANSI SQL for a low learning curve 
- focused on taking advantage of being natively on cloud 

Weaknesses:
- as with every data warehouse, they are expensive 
- competes with Redshift which is more widely used and better documented 

References:
- [1] http://www.bityota.com/product/
- [2] http://www.esg-global.com/blogs/the-week-that-waas-bityota-and-redshift/
- [3] http://www.businessinsider.com/bityota-amazon-data-warehouse-2012-11
- [4] http://cloudcomputingeurope.sys-con.com/node/2466082




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



**Exasol**  
*C5*  
What:
- database management software company with the primary product of EXASolution 
- in memory, column oriented, relational database management software 
- compresses data heavily 

Strengths:
- doesn't need to be configured/tuned as the database performs self optimization 
- known for really good performance from the columnar orientation + in memory compression 
- perks of column based databases is that you can avoid the need for entire table scans and pre aggregation of data 

Weaknesses:
- relies on their being a lot of RAM 
- implicit assumption that the queries you are running are on data stored in RAM 
- proprietary system gives you little flexibility; you need to run the data warehouse on top of EXACluster OS (the company's own operating system)

References:
- [1] http://www.exasol.com/en/
- [2] http://en.wikipedia.org/wiki/EXASOL
- [3] http://www.informationweek.com/software/information-management/comparing-vertica-paraccel-and-exasol/d/d-id/1071118?
- [4] http://www.it-director.com/technology/data_mgmt/content.php?cid=10541




