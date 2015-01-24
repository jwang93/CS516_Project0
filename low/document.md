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


