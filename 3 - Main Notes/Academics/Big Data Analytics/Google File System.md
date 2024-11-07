
2024-11-06 04:21

Status: #Finished  

Tags: [[big data]] [[storage]] 

# Google File System

GFS is basically Hadoop with additional features and improved performance.

There are 2 unique operations performed in GFS:
1. **Snapshot Operation**: Creates copy of a file at a low cost
2. **Record Operation**: Allows multiple users to append to the same file concurrently

GFS mainly manages 2 types of data.
1. File Metadata
2. File Data

Like HDFS, GFS also consists of a single master node and several chunk servers. The only difference is that unlike in HDFS, the client won't have to interact with MasterNode every time it wants to modify any file. 

#### How GFS works?
1. Client makes request to MasterNode
2. MasterNode provides client with the metadata of the file chunk it wants to access/modify
3. Now that the client has the metadata, next time it wants to make any changes, it'll directly access the file without having to interact with the MasterNode again.
4. Client makes changes in the primary replica.
5. The primary replica forwards the changes to the secondary replicas.

GFS has only single MasterNode (No secondary MasterNode). Incase of failure, the MasterNode automatically restarts and uses *"checkpoint"* to restore the last state of the MasterNode. Checkpoint is basically like a snapshot but for the metadata only. 







#### References
[[GFS University Lecture Big Data Analytics.pdf]]