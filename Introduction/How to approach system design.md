
### Step 1 : Outline use cases, constraints and assumptions.

Gather requirements and scope of the problem. Ask question to clarify use cases and constraints. Discuss assumptions 
* Who is going to use it ?
* How they are going to use it ?
* How many users are there ?
* What does the system do ?
* What are the inputs and outputs of the system ?
* How much data do we expect to handle ?
* How many request per second do we expect ?
* What is the expected read to write ratio ?

### Step 2 : Create a high level design

Outline a high level design with all important components 
* Sketch the  main component and connections.
* Justify your ideas. 

### Step 3 : Design the core components


Dive into details for each core component. For example, if you were asked to "design a url shortening service" discuss : 

* Generating and storing a hash of full uri
	* MD5 or Base62
	* Hash collisions
	* SQL or NOSQL
	* Database Schema
* Translating a hashed url to the full url 
	* Database Lookup
* API and object oriented design 

### Step 4 : Scale the design

Identify and address the bottlenecks. For example, do you need the following to address scalability issues ?

* LoadBalancer
* Horizontal scaling 
* Caching 
* Database sharding