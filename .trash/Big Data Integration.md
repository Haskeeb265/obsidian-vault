
2024-11-06 05:35

Status: #Finished

Tags: [[big data]] [[data]] [[academics]] 

# Big Data Integration

Big data integration is the process of combining, managing, and organizing large volumes of data for analytical purposes. 

Following are the 3 major steps we take for data integration:
1. **Schema Alignment**: Matching or mapping the schemas of data from different sources
2. **Record Linkage**: Identifying records that refer to the same entity across different datasets
3. **Data Fusion**: Combining data from different sources to create a more complete and comprehensible dataset

## Schema Alignment:

Following are the 3 steps of Schema alignment:

1. **Mediated Schema**
   >Mediated Schema is a schema which doesn't belong to any source. Rather it combines two or more schemas together and form a unique schema.
2. **Attribute marching**
   >Identifying which attributes are same even though they might be under different table names.
3. **Schema Mapping**
   >How the data should be mapped from the sources to the unified schema.   

## Record Linkage:

Following are the 3 steps of record linkage:

1. **Blocking**:
   >Makes small blocks of similar records 
2. **Pairwise Matching**:
   >Compares all record pairs in a block
3. **Clustering**:
   >Groups sets of records into entities
   
## Data Fusion:

Following are the 3 steps of Data Fusion:

1. **Voting**:
   >Ensures conflicting of differing information is resolved. Select the most frequent and accurate values
1. **Source Quality**:
   >Prioritize dataset with a more credible source
4. **Copy Detection**:
   >Detect any redundant records. Removes duplicate records linking to the same entity.

#### References
[[Big Data Integration University Lecture.pdf]]