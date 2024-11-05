
2024-11-06 04:21

Status: #InProgress 

Tags: [[big data]] [[storage]] 

# Google File System

GFS is basically Hadoop with additional features and improved performance.

There are 2 unique operations performed in GFS:
1. **Snapshot Operation**: Creates copy of a file at a low cost
2. **Record Operation**: Allows multiple users to append to the same file concurrently

GFS mainly manages 2 types of data.
1. File Metadata
2. File Data

Like HDFS, GFS also consists of a single master node and several chunk servers




#### References
[[GFS University Lecture Big Data Analytics.pdf]]