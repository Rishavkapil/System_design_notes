

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

Taking a user database as an example, as the number of users increases, more shards are added to the cluster. 

Similar to the advantage of federation, sharding results in less read and write traffic, less replication, and more cache hits. 



## What is the difference between Database Sharding and Replication ?

**Core Idea**

**Sharding :** Split data across multiple nodes(horizontal partitioning)

**Replication:** Copy data across multiple nodes(redundancy and high availability)

Database Sharding scales horizontally by splitting data. 

Sharding breaks large database into multiple smaller, independent databases(called shards). 

Each shard contains a different subset of data. 


## Federation

Federation (or functional partitioning), splits up database by function. For example, instead of a single monolithic database, you could have three databases : forums, users, and products, resulting in less read and write traffic to each database and therefore less replication lag. 


It refers to splitting data across multiple independent databases, where each database is autonomous and responsible for a specific domain, but they are logically combined and can be queried as a single system. 

**Why federation exists ?**

Instead of one giant monolithic database, different teams/services manage their own database that fits their domain, improving scalability and independence. 


Now you'll getting confused between sharding and federation. Yes, mostly they are same but they differ in how they split the data. 

* **Sharding:** Same schema, split by rows/partitions of data. 
* **Federation:** Different Schema, split by domains/services.
