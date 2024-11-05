
2024-11-05 16:53

Status: #InProgress

Tags: [[big data]] [[storage]] 

# Hadoop HDFS

Hadoop is an open source framework which allows us to store and process large amount of data in a parallel and distributed manner. It supports data-intensive distributed applications

**HDFS** and **MapReduce** are two main components of Hadoop. HDFS is the primary data storage system whereas the MapReduce is the processing unit of Hadoop

Hadoop was designed to answer the question:
>**"How to process big data with reasonable cost and time?"**

#### Goals of Hadoop
- Facilitate storage and processing of large and rapidly growing datasets
- High scalability and availability
- Use cheap hardware with little redundancy
- Fault tolerant
- **Move computation rather than data**

#### Architecture of Hadoop
![[Pasted image 20241105173914.png]]

> [!NOTE] Hadoop Architecture 
> - **NameNode**: The primary job of NameNode is to manage the metadata of all the files and directories. The NameNode also knows which DataNode holds the data blocks of each file.
>   The **MetaData** is data about the data. The activity 
> - **DataNode**: 




#### References
[[Lecture 2 Big Data Analytics Hadoop HDFS.pdf]]