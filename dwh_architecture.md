# What is a Hadoop ecosystem?
It consists of two scalable components:
- Data Storage: **HDFS** --> Hadoop Data File System or cloud storage: such as buckets.
- Processing API: **MapReduce**

It is gone far beyond the intial two pieces. 

![image](https://github.com/mahmoudabderahman/hadoop-distributed-systems/assets/30775657/b7719946-723f-4219-b423-88d6ee4dc56b)

## Where Hadoop Shines
- **Scalability (Partitioning)** -> Commodity hardware for data storage.
- **Flexibility (Availability)** -> Commodity hardware for distributed processing.

### Business Areas for Hadoop
- **Understanding behavioral data** -> Hadoop is used in areas like risk modeling, customer churn analysis, and recommendation engines, enabling analysis of behavioral data over transactional data.


### Dataproc
Dataproc is a managed Spark and Hadoop service that lets you take advantage of open source data tools for batch processing, querying, streaming, and machine learning. Dataproc automation helps you create clusters quickly, manage them easily, and save money by turning clusters off when you don't need them. With less time and money spent on administration, you can focus on your jobs and your data.

### Dataproc Metastore
Dataproc Metastore is a fully managed Apache Hive metastore (HMS) that runs on Google Cloud. An (HMS) is the established standard in the open source big data ecosystem for managing technical metadata, such as schemas, partitions, and column statistics in a relational database.

Dataproc Metastore is highly available, autohealing, and serverless. Use it to manage data lake metadata and provide interoperability between the various data processing engines and tools that you're using.

# Physical Cluster Architecture
![image](https://github.com/mahmoudabderahman/hadoop-distributed-systems/assets/30775657/eda64bad-323b-4a7e-a458-b5aa54c71587)

## Understand Hadoop and JVMs
- Hadoop processes run in separate JVMs (daemons)
- JVMs do not share state - functional progrmaming mdoel
- JVM process details differ between Hadoop versions

## Hadoop File Systems: HDFS
- HDFS (Hadoop Distributed File System): Distributed (by default, replicated three times) or pseudo-distributed (for testing, it is a single node).
- Regular File System: Standalone
- Cloud File Systems

# What is a Data Model?
- An abstract model that organizes elements of data.
- It describtes the objects, entities, and data structure properties, semantic, and constraint.
- It formalizes the relationship between entities.
- It describes how the application (report) API data manipulation.
- It describes the conceptual design of a business or an application with its flow, logic, semantic information (rules), and how things are done.

![image](https://github.com/mahmoudabderahman/hadoop-distributed-systems/assets/30775657/1418b217-b60e-4448-8c0a-4f7b44744a55)
