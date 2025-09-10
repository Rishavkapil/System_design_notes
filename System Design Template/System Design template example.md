
## 1. Feature Expectation

* Use cases
* Scenarios that will not be covered.
* who will use
* How many will use
* usage patterns

## 2. Estimations 

* Throughput
* Latency expected from the system.
* Read/Write Ratio.
* Traffic Estimates
* Storage Estimates
* Memory Estimates

## 3. Design Goals

* Latency and throughput requirements
* Consistency vs Availability 
## 4. High Level Design 

* APIs for READ/Write scenarios for crucial components
* Database Schema
* Basic Algorithm
* High Level design for read/write scenario.

## 5. Deep Dive

* Scaling the Algorithm 
* Scaling Individual components 
* Think about following components : 
	* DNS
	* CDN
	* Load Balancer
	* Reverse proxy
	* DB
	* Caches
	* Communication


## 6. Justify

* Throughput of each layer
* Latency caused between each layer
* Overall latency justification. 