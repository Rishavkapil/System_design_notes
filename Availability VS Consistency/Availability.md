The Availability of distributed system is the percentage of time in a given period that a system is available to perform its task and function under normal conditions. 


### How is availability measured 

We can measure the availability of a distributed as a percentage of system's uptime . i.e dividing total uptime by total uptime and total downtime. 

```
Availability = total uptime / (total uptime + total downtime)
```


### The Nine's of availability 
We usually measure availability in terms of Nines rather than percentages. If the availability is 99.00% , then it is said to have "2 nines" of availability , and if it 99.9% , then it is called "3 nines" and so on. A system with 5 nines (i.e 99.999%) is a Gold Standard of Availability. 


| Availability %      | Downtime/year | Downtime/month | Downtime/weak |
| ------------------- | ------------- | -------------- | ------------- |
| 90%(one nine)       | 36.53 days    | 72 hours       | 16.8 hours    |
| 99%(two nines)      | 3.53 days     | 7.20 hours     | 1.68 hours    |
| 99.9% (three nines) | 8.77 hours    | 43.8 minutes   | 10.1 minutes  |
| 99.99% (four nines) | 52.6 minutes  | 4.32 minutes   | 1.01 minutes  |
| 99.999%(five nines) | 5.25 minutes  | 25.9 seconds   | 6.05 seconds  |


### How do we achieve high availability 

To increase availability , we can use redundancy by duplicating or adding additional components(server or storages)
