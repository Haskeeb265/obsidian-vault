
2024-11-05 16:53

Status: #Finished

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

#### Architecture of HDFS

![[HDFS Architecture.png]]

> [!NOTE] Hadoop Architecture 
> - **NameNode**: The primary job of NameNode is to manage the metadata of all the files and directories. The NameNode also knows which DataNode holds the data blocks of each file.
>   
>   The **MetaData** is data about the data. User logs, information regarding the stored data; where its stored, how big it is and so on. NameNode uses this information to find the closest DataNode for faster communication. NameNode also instructs DataNode regarding creation, deletion, and replication.
>   
>   For Fault-Tolerance, NameNode uses *heartbeats* of the DataNode and manages the replication (by default its 3) incase any block fails. Heartbeat is basically a signal from the DataNode to the NameNode which reassures NameNode that that DataNode is available for service
>   
>   The secondary NameNode is used to achieve availability. The secondary NameNode synchronizes with the primary NameNode and takes over incase the MasterNode fails causing minimum downtime 
>   
>   Usually the 1st replica is stored in the same node as the client making request. The 2nd replica is stored in a different rack incase the first rack fails. The 3rd replica is stored in the same rack as the 1st one allowing fast communication
>   
> - **DataNode**: Responsible for the actual storage of the data. DataNode sends *heartbeats* to the NameNode to let it know that its available for service. The DataNode also sends a *block report*. This stores the list of all the blocks stored in the DataNode. It sends this report to NameNode every once an hour so that NameNode can quickly identify which blocks were lost incase of a DataNode failure.


#### JobTracker and TaskTracker 

JobTracker is the MasterNode which runs in the MapReduce engine. The JobTracker overlooks all the MapReduce executions. It coordinates and distributes tasks to the TaskTracker. JobTracker accepts requests from the client and the splits them into smaller tasks. Then JobTracker assigns those tasks to the available TaskTracker nodes. The TaskTracker is a worker node which is assigned tasks by the JobTracker. The TaskTracker runs both Map and Reduce on the data assigned by the JobTracker


#### MapReduce

MapReduce is the processing unit of Hadoop. It can be broken down into 2 functions:
1. **Map()**
2. **Reduce()**

The **Map()** takes input (set of data) and breaks it down into *tuples* (key value pairs). Once the tuples are made, they're shuffled and sorted into values with the same key. The **Reduce()** takes these shuffled tuples as an input *(intermediate output)* and combines the values with the same key applying functions like aggregation and then delivers the output.

The **MapReduce** has 3 main components:
1. Driver Code (For Initialization)
2. Mapper (For Transformation)
3. Reducer (For Aggregation)

MapReduce processes the data in parallel by dividing the job into a set of independent tasks (sub-jobs)

Since Hadoop has a major drawback of cross-switch networks, MapReduce introduced the concept of **Data-Locality** which is basically moving the computational operations closer to the data instead of the other way around.


#### Applications of Hadoop:
- Advertisement (Mining user behavior to generate personalized ads)
- Searching (Group related docs)
- Security (searching for odd or uncommon patterns)
#### References
[[HDFS University Lecture.pdf]]
[[MapReduce University Lecture.pdf]]