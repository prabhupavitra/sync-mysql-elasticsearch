### MySQL Database Migration and Synchronization with Elasticsearch

A majority of companies believe that leveraging customer-data is the key to gaining competitive edge. In other words, the more customers you have, more data you are able to gather and analyze, which then allows you to build a better product. 
For this reason, leading companies invest heavily in database development and building other data infrastructure. More often than not, companies build their essential functionalities around relational databases. This is due to the fact that, relational databases have strict data integrity procedures that keep the integrity of crucial data throughout all database procedures and operations. However, traditional databases are ineffective for the purposes of analytics and implementing full-text search capabilities. Therefore, there is a need for a search engine that allows us to store, search, and analyze huge volumes of data quickly and in near real-time and give back answers in milliseconds.  

Elasticsearch is the world’s leading free and open search and analytics solution at the heart of the Elastic Stack that provides a rapid full-text search over millions of documents in near real-time. It is built on Apache Lucene and developed in Java. Logstash and Beats facilitate collecting, aggregating, and enriching your data and storing it in Elasticsearch. Kibana enables you to interactively explore, visualize, and share insights into your data and manage and monitor the stack. Elasticsearch is where the indexing, search, and analysis magic happens.</span>   

In order to take advantage of the robust search capabilities offered by Elasticsearch, many businesses will deploy Elasticsearch alongside existing relational databases. In this project, we explore the ELK stack and use Logstash to create a data pipe linking Elasticsearch to MySQL in order to build an index from scratch and keep Elasticsearch synchronized with MySQL database using Logstash and JDBC. The scenario is that, our legacy system uses MySQL database and we have a requirement where we need to have a heavy search and we have decided to move to Elasticsearch. We will still stick to our MySQL database as a primary database for application-db transactions and use ElasticSearch as a secondary data store for the requirements where we need to have the heavy search.


#### Dataset

The submissions data set contains summary information about an entire EDGAR submission. Some fields were sourced directly from EDGAR submission information, while other columns of data were sourced from the Interactive Data attachments of the submission. Note: EDGAR derived fields represent the most recent EDGAR assignment as of a given filing’s submission date and do not necessarily represent the most current assignments. 
To access the complete submission files for a given filing, please see the [SEC EDGAR website](https://www.sec.gov).
