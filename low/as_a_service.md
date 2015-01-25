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




**Actian Ingres**  
*B3*  
What:  
- database management system
- used for enterprise 
- open source, SQL 

Strengths:  
- has out of the box spatial management  
- traditional database features - ACID, transactions
- open source 

Weaknesses:  
- bit archaic 
- fact that it uses SQL creates a barrier to use 

References:  
- [1] http://www.actian.com/products/operational-databases/ingres/
- [2] https://www.princeton.edu/~achaney/tmve/wiki100k/docs/Ingres_%28database%29.html 





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



**Actian PSQL**  
*B5*  
What:
- yet another database management system from Actian

Strengths:  
- has the ability to be embedded making it good for packaged business apps 
- very low maintenance - they call it "Zero DBA"

Weaknesses:  
- expensive 
- limited functionality compared to a more involved system 

References:  
- [1] http://www.actian.com/products/operational-databases/psql/



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




**AWS ElastiCache with Redis**  
*E2*  
What: 
- same thing as ElastiCache, just that you are using Redis rather than Memcached as the memory caching service 

Strengths: 
- get the same abstraction of not having to manually set up Redis 

Weaknesses:  
- cost 

References:  
- [1] http://aws.amazon.com/elasticache/
- [2] http://stackoverflow.com/questions/21175941/redis-amazon-ec2-vs-elasticache



**AWS Kinesis**  
*A2*  
What: 
- fully managed cloud based service for realtime processing of large data streams (think competitor to Kafka, Spark Streaming)

Strengths:  
- like most of these AWS services (called managed services), it is very easy to set up and get started
- elasticity allows for easy scaling 

Weaknesses:  
- software as a service means you will need to pay money, which sucks because there are open source alternatives such as Kafka 
- every application consists of just one procedure so you can't do complex stream processing like in Storm 

References:  
- [1] http://aws.amazon.com/kinesis/
- [2] http://www.quora.com/What-can-you-do-with-Amazon-Kinesis
- [3] http://gworley3.blogspot.com/2013/11/amazon-kinesis-compared-to-storm.html
- [4] http://diamondstream.com/amazon-kinesis-big-real-time-data-processing-solution/



**AWS SimpleDB**  
*E2*  
What:
- Amazon's non relational data store 

Strengths:  
- managed multiple copies of your data in various geographic locations which helps to ensure reliability 
- simplicity that comes from not being a relational database: don't have to worry about schema and adhering to strict rules 
- cheap set up costs and the ability to pay as you go makes it ideal for startups 

Weaknesses:  
- missing a couple of standard SQL operators like JOIN or IN 
- relatively high cost given how easy it is to set up a standalone DB
- your data is under Amazon which can potentially lead to privacy issues (note that this is the case for all of these AWS services)

References:  
- [1] http://highscalability.com/current-pros-and-cons-list-simpledb
- [2] http://aws.amazon.com/simpledb/


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


**ClearDB**  
*D5*  
What:
- database for MySQL applications 
- impressive customer set of Microsoft and salesforce 

Strengths:
- fault tolerant, which means that if a component fails, a backup system can come back up immediately with no need for human maintenance 
- can support database size up to 10GB 

Weaknesses:
- doesn't have the community of Amazon RDS 
- easy to set up (< 1 minute) but you need to use one of their partners: Heroku, Appfog, Azure cloud 

References:
- [1] https://www.cleardb.com/
- [2] http://w3facility.org/question/xeround-vs-cleardb-hosted-mysql-pros-and-cons/
- [3] http://www.sitepoint.com/database-as-a-service-mysql-in-the-cloud/



**Cloudant**  
*E2*  
What:
- fully managed NoSQL Database as a service 
- acquired and now managed by IBM 
- ** NoSQL DBs can't do joins the way a relational database does, NoSQL DB is really good for document stores **

Strengths:
- requires no configuration / easy set up
- embeddable, easy to use alongside ElasticSearch
- scales better than MongoDB and more stable 
- queries in JavaScript and REST

Weaknesses:
- can't perform joins (and other downsides of NoSQL)
- expensive 

References:
- [1] https://cloudant.com/
- [2] http://en.wikipedia.org/wiki/Cloudant
- [3] http://blog.postmarkapp.com/post/37338222496/bye-mongodb-hello-cloudant
- [4] http://vschart.com/compare/cloudant/vs/dynamo-db
- [5] https://getsatisfaction.com/application_craft/topics/anyone_have_experience_with_cloudant_couchdb



**CloudBird**  
*D2*  
What:
- RavenDB in the cloud

Strengths:
- RavenDB is built for .NET programming (can also support Java and HTML)
- schema free, scalable, transactional 
- good for OLTP (fast, datatore feel)

Weaknesses:
- limited language support results in limited features 
- not a database as a service means that you need to manually configure it yourself 

References:
- [1] http://ravendb.net/
- [2] http://db-engines.com/en/system/MongoDB%3BRavenDB
- [3] http://ayende.com/blog/136196/when-should-you-use-ravendb


**Compose**  
*D2*  
What:
- company that offers production ready, cloud hosted services for: mongodb, elasticsearch, redis, postgresql 

Strengths:
- made for developers who don't want to invest time in setting up their own services 
- offers a cloud based solution, so don't need to worry about managing the hardware
- these people are professionals and know exactly how to manage your data 

Weaknesses:
- costs money 

References:
- [1] https://www.compose.io/
- [2] http://www.quora.com/As-a-website-developer-should-i-manage-database-myself-or-give-control-of-this-important-piece-of-my-website-to-someone-else-who-in-fact-is-just-another-startup-MongoHQ-compose-io-Note-I-have-been-playing-around-with-MongoDb-and-really-liked-using-it-but-Im-not-a-master-of-this-domain




**Database.com**  
*D5*  
What:
- cloud database run by Salesforce
- opening up the database it uses to power Salesforce CRM and providing developer tools on top of that 

Strengths:
- many of the similar advantages one gets with AWS 
- seems to be a similar product to the Oracle database but cheaper 
- great for the smaller applicationd developers, mobile developers who are willing to try something new 

Weaknesses:
- security, do you want to hand over your data to another third party?
- lose complete control over your data from a mangement perspective 

References:
- [1] http://www.salesforce.com/platform/database/?d=70130000000lll1
- [2] http://www.quora.com/What-are-the-pros-cons-of-hosting-a-database-on-Salesforces-Database-com-vs-Amazons-Relational-Database-Service
- [3] http://www.infoworld.com/article/2624989/cloud-computing/what-salesforce-s-database-com-really-means.html



**EnterpriseDB**  
*B3*  
What:
- enterprise software, solutions, tools for PostgreSQL 

Strengths:
- supports Postgres which has its own slew of advantages over MySQL 
- comes with a bunch of services like consulting, data management
- more features for enterprise systems are in Postgres 

Weaknesses:
- supports a unique use case of PostgreSQL 
- makes it harder for people using MySQL systems to migrate
- costs money 

References:
- [1] http://www.enterprisedb.com/
- [2] http://en.wikipedia.org/wiki/EnterpriseDB
- [3] http://www.enterprisedb.com/solutions/mysql-vs-postgresql/why-move-mysql-postgres-plus




