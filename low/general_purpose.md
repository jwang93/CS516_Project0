
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



**Actian Versant**   
*E1*  
What:
- object database 
- Actian acquired Versant to expand its data analytics offerings 

Strengths:  
- handling more complex object models 
- NoSQL
- focused on real-time analytics 

Weaknesses:  
- steep technical knowledge required to use

References:  
- [1] http://www.actian.com/products/
- [2] http://globenewswire.com/news-release/2012/11/21/506794/10013391/en/Versant-Agrees-to-be-Acquired-by-Actian-for-13-00-per-Share.html
- [3] http://en.wikipedia.org/wiki/Versant_Object_Database



**Adabas**  
*D1*  
What:
- database management system from Software AG
- stands for Adaptable Database System 
- it is NoSQL, not relational 

Strengths:  
- performance (esp. on mainframes) 
- inverted list architecture makes it faster than traditional relational DB's 

Weaknesses:  
- doesn't do data compression or encryption like DB3 does 
- doesn't have the referential integrity that Oracle MySQL has 

References:  
- [1] http://tech.forums.softwareag.com/techjforum/posts/list/24345.page
- [2] http://database-management.findthebest-sw.com/compare/2-9/ADABAS-vs-DB3 
- [3] http://database-management.findthebest-sw.com/compare/2-30/ADABAS-vs-MySQL


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



**Documentum xDB**  
*C1*  
What:
- database out of EMC, interesting because it is a native XML database 
- not relational 

Strengths:
- many of the pros of NoSQL systems such as being able to store more complex objects
- good at managing XML structures
- native XML means that the underlying data is stored as XML so it does not need to convert from XML to a different data type
- this increases efficiency and improves performance 

Weaknesses:
- very niche use case of only XML
- peoeple are moving away from XML because it is too verbose and picking formats such as JSON 

References:
- [1] http://www.emc.com/products/detail/software2/documentum-xdb.htm
- [2] http://en.wikipedia.org/wiki/XML_database



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



