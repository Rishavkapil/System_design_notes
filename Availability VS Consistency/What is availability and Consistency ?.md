
Availability refers to the ability of the system to provide its services to clients even in the presence of failures . This is often measured in terms of percentage of time that the system is up and running. 

Consistency on the other hand refers to the property that all clients see the same data at the same time. This is important for maintaining the integrity of the data stored in the system. 


### Consistency 
Every read receives most recent write or an error . 

### Availability 
Every request receives a response, without guarantee that it contains most recent version of data. 

### Partition Tolerance 
The system continues to operate despite arbitrary partitioning due to network failures. 