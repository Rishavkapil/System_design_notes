

## Replication

Replication is the process of copying data from one database to another. 

Replication is used to increase availability and scalability of databases. 

There are two main types of replication master-slave and master-master. 

#### Master-Slave Replication 

The master serves read and writes, replicating writes to one or more slaves , which serve only reads. Slaves also replicate to additional slaves in a tree-like fashion. 

If master goes offline, the system can continue to operate in read-only mode until a slave is promoted to a master or a new master is provisioned. 

#### Master-Master Replication

Both masters serve reads and writes and coordinate with each other on writes. If either master goes down, the system can contribute to operate with both reads and writes. 




## Sharding

Sharding distributes data across different databases such that each database can only manage a subset of the data. 