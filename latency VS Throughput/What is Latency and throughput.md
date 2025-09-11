
Latency and throughput are two important measures of a system's performance. 

* **Latency** refers to the point the amount of time it takes for a system to respond to a request. 


* **Throughput** refers to the number of request that a system can handle at the same time. 

Latency is a measure of how long it takes for a system to complete a task or process data. 

High Latency can lead to slow performance , while low latency can result in faster performance.  

Latency can be caused by various factors  eg. network i.e time it takes for data to travel through the network(more hops, high latency), network congestion, inefficient algorithms, load on the resources and so on. 


### Throughput 

Throughput refers to the number of requests a system can handle at a same time. It is often measured in requests per second, 

Throughput is often measured in requests per second, or requests per transactions

Throughput can be limited by various factors , such as capacity of the system involved , number of available resources and efficiency of the algorithm used to process the data. 


## Example 

One real world example to show the relationship between both is the design of the web server. In this case, the goal is to balance the need of low latency(so that pages load quickly) with the need for high throughput ( so that server can handle many requests at the same time).

One way to handle throughput is to add more servers to the system, which allows system to handle more requests simultaneously . However, this can lead to increased latency, as the requests may need to be routed to different servers and the data may need to be replicated across those servers. 


Another way to increase the throughput is to optimize the web server software to handle more request at the same time. However , this can also lead to increased latency , as the server may need to use more resources to keep up with the increased demand. 


In this case, the system design needs to balance these trade offs to find the right balance between low latency and high throughput. This may involve using caching and load balancing techniques to minimize the latency while increasing throughput. 