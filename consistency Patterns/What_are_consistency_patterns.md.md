
Consistency patters refers to the ways in which data is stored and managed in a distributed systems, and how data is made available to the users and applications. 
There are three main types of consistency patterns : 

* Strong Consistency 
* Weak Consistency 
* Eventual Consistency 


## What are distributed Systems ?

 A Distributed system is a system that consists of more than one components, and each component is responsible for one part of the application.


### Example of distributed System 
Imagine we have an e-commerce application where we are selling books. This application may consist of multiple components . For example, one might be responsible for accounts, one might be responsible for payments , one might be responsible for storing orders, etc and so on. 

![[Pasted image 20250911113520.png]]

Now , if a user buys a book, there might be different services involved in placing your order; order service for storing the order, payment service for handling the payments etc. 

This is an example of distributed systems, an application that consist of multiple components , each of which is responsible for different part of application. 


## Why Consistency is important ?

When working with distributed systems, we need to think about managing the data across different servers. If we take the above example of the e-commerce application, we can see that the inventory service must have up-to-date stock information for the ordered items if the user places an order. Now, there might be two different users looking at the same book. Now imagine if one of the customers places a successful order, and before the inventory service can update the stock, the second customer also places the order for the same book. In that case, when the inventory wasn’t updated, we will have the wrong stock information when the second order was placed, i.e., the ordered book may or may not be available in stock. This is where different consistency patterns come into play. They help ensure that the data is consistent across the application.



## Consistency patterns 

Consistency patterns refers to the ways in which data is stored and managed in a distributed systems and how data is made available to the users and applications. 


#### Strong Consistency 
After an update is made to the data, it will be immediately visible to any subsequent read operations. The data is replicated in a synchronous manner, ensuring that all copies of data are updated at the same time. 

In Strong Consistency systems, any updates to some data are immediately propagated to all locations. This ensures that all locations have same version of data, but it also means that system is not highly available and has high latency. 



#### Weak Consistency
After an update is made to the data, it is not guaranteed that any subsequent read operation will immediately reflect the changes made. The read may or may not see the recent write. 

In weakly consistent systems, updates to the data may not be immediately propagated. This can lead to inconsistencies and conflicts between different versions of the data, but it also allows for high availability and low latency . 

