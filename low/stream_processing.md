
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


**DataTorrent**  
*A2*  
What:
- realtime streaming platform for enterprise 
- similar to Apache Storm 

Strengths:
- handle realtime processing 
- can support "exactly onces" semantics which is when you process the data only once (a problem that a lot of realtime systems have)
- can support a number of data sources 
- runtime operations are managed for you: scaling, resource optimization, availability, etc 

Weaknesses:
- enterprise product you will have to pay for 
- not that much of a community around it (probably not needed since all the maintenance and setup is handled for you) 

References:
- [1] https://www.datatorrent.com/
- [2] http://www.datanami.com/2014/04/23/crossing_the_big_data_stream_with_datatorrent/
- [3] http://hortonworks.com/partner/datatorrent/
- [4] https://mybigdatajourney.wordpress.com/2014/07/24/open-source-storm-vs-commercially-available-data-torrent/



**FeedZai**  
*A2*  
What:
- big data company trying to detect fraud in commerce 
- uses machine learning on top of its massive amount of data 

Strengths:
- handling fraud means insights need to be uncovered quickly, which is why FeedZai is big on realtime processing 

Weaknesses:

References:
- [1] https://www.feedzai.com/home/big-data-insight/
- [2] http://en.wikipedia.org/wiki/Feedzai
- [3] http://www.forbes.com/sites/tomgroenfeldt/2014/02/03/feedzai-brings-machine-learning-and-data-science-to-payment-fraud/


