Failover is the availability pattern that is used to ensure that a system can continue to function in the event of failure. It involves having a backup component or system, that can take over in the event of failure. 

In failover systems, there is a primary component that is responsible for handling requests , and a secondary (or backup ) component is on stand by. The primary component is monitored for failures and if it fails , the secondary component is activated to take over duties. 

Failover can be implemented in varioius ways such as active-passive , active-active. 

### Active Passive 
With Active-Passive Failover , heartbeats are sent between active and passive server on standby. If the heartbeat is interrupted , the passive server takes over the active's IP address and resumes services. 

### Active Active
In active active , both servers are  managing traffic , spreading the load between them. 
If the servers are public facing, then DNS would need to know about the public ips of both servers. If the serers are internal facing , application logic would need to know about both the servers. 