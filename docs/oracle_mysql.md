#  MySQL Database Cloud Service

The two key defining characteristics of the MySQL Database Cloud Service are the **high availability** feature, which you should definitely use for production and then **HeatWave**, which lets you do both OLAP and OLTP transactions using the MySQL Database Cloud Service. 

## High Availability

High availability basically gives you that fault tolerance. It has a lot of benefits like automatic failover, increased uptime, zero data loss. 

With a standalone option, you get a single instance MySQL DB systems back ended by the resilient and secure OCI block volume. This option is good for dev and test and development environment. But if you're running in production, you really want to go with the high availability option. This option enables applications to meet higher uptime requirements and the zero data loss tolerance.

When you select the high availability option, MySQL DB system with **three instances** is provisioned across different availability domains or different fault domains. The data is replicated among the instances. 

## Heatwave

HeatWave is a new integrated high performance in memory query accelerator for MySQL Database Service that accelerates MySQL performance by order of magnitude for analytics and transaction queries. HeatWave scales out to thousands of cores.

MySQL Database Service with HeatWave is the only service available in the market that enables database admins and app developers to run both OLTP and OLAP workloads directly from their MySQL database. This eliminates the need for complex, time consuming, and expensive data movement, and integration with a separate analytics database. This service is optimized for and exclusively available in Oracle Cloud Infrastructure.

MySQL HeatWave uses an **in-memory data storage** mechanism to provide high-performance query execution. It achieves this by storing the data in a columnar format in-memory, which allows for faster access and processing of data during query execution, especially for OLAP workloads.

MySQL HeatWave is an integrated query accelerator for the MySQL Database service in Oracle Cloud Infrastructure. It significantly boosts the performance of MySQL, enabling it to efficiently run OLAP (Online Analytical Processing) queries, which are complex queries that analyze large amounts of data to uncover business insights.