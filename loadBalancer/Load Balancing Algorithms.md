A Load Balancer is a hardware or software device that keeps any one server from becoming overloaded. A Load Balancing Algorithm is a logic that a load balancer uses to distribute network traffic between servers. 



There are two primary approaches to load balancing. *Dynamic load balancing* uses algorithms that take into account current state of each server and distribute traffic accordingly. 

*Static Load Balancing* distributes traffic without making these adjustments.
Some static algorithms sends equal amount of traffic to each server in a group, either in a specified order or at random. 


### Dynamic Load Balancing Algorithms

* *Least Connections* : Checks which server has the fewest connections open at a time and send traffic to that servers. This assumes all connections require roughly equal processing power. 

* *Weighted Least Connections:*  Gives administrators the ability to assign different wights to each server, assuming that some servers can handle more connections than others. 

* *Weighted Response time:* Averages Response time of each server, and combines that with the number of connections each server has open to determine where to send traffic. By sending traffic to servers with quickest response time, the algorithm ensures faster service for users. 

* *Resource Based :* Distributes load based on what resource each server has available at the time. Specialized software (called an "agent" ) running on each server measures that server's available CPU and memory, and the load balancer queries the agent before distributing traffic to that server. 

## Static Load Balancing Algorithms

* *Round Robin :* distributes traffic to a list of servers in rotation using DNS. A authoritative nameserver will have list of A records for a domain and provides a different one in response to each DNS query. 

* *Weighted Round Robin :*  Allows administrator to assign different weights to each server. 