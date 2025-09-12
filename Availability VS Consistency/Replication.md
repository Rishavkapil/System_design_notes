Replication is an availability pattern that involves having multiple copies of the same data stored in different locations. In the event of a failure, the data can be retrieved from different locations. 

There are two main types of replication master-master replication  and Master Slave replication. 


### Master-Master Replication

In this type of Replication, multiple servers are configured as "masters", and each one can accept read and write operations. This allows high availability and allows any of the servers to take over if one of them fails. 

However, this type of replication can lead to conflicts if multiple servers update the data at the same time, so conflict resolution is needed to handle this. 

### Master-Slave Replication

In this type of replication, one server is designated as the "master", and handles all write operations, while multiple "slave" servers handle read operations. If the master fails, one of the slave can be promoted as 