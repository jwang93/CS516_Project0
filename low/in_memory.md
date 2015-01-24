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


**Aerospike**  
*C2*  
What:
- optimized for flash, in-memory database
- NoSQL database 

Strengths:  
- flash optimized, so should be super fast with a hybrid RAM/Flash storage architecture
- good for concurrent, low latency, more read than write 

Weaknesses: 
- jobs with high write volume 
- can't operate on non-SSDs which makes it more expensive than something like Cassandra were you can store your keys on disk 

References:  
- [1] http://www.aerospike.com/
- [2] http://www.aerospike.com/about-aerospike/
- [3] http://stackoverflow.com/questions/25443933/comparison-aerospike-vs-cassandra



**Altibase HDB**   
*D3*  
What:
- hybrid in memory database, hence the name HDB developed by altibase 
- utilizes spatial indexing 

Strengths:  
- purported to be very fast (although this is from Altibase)
- lot of features that competitors don't have such as - SQL Interpreter, Java Support, Real Time Access

Weaknesses:  

References:  
- [1] http://altibase.com/in-memory-database-hybrid-products/hdbtm-hybrid-dbms/
- [2] http://database-management.findthebest-sw.com/compare/5-36/ALTIBASE-HDB-vs-Oracle 
