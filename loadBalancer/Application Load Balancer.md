
## How an Application Load Balancer works ?

ALB distributes traffic across multiple targets, such as EC2 instances. 

For example , an e-commerce application has a product directory, shopping cart and checkout function. 

Your e-commerce website has different features : 

* Browsing products(images, videos)
* Shopping Cart (needs keeping user sessions)
* Checkout (secure , API-heavy)

Different parts of website need different servers. 
So the ALB decides : 

* "Oh, this request is just looking at product images" -> send it to product servers. 
* "This request is updating the shopping cart " -> send it to cart servers. 
This way you don't overload one single server with everything. 

Yes, reverse proxy also works the same but ALB does much more than that for increasing / decreasing the number of instance depending upon the load. 


### What is a Listener ?

A listener is the "ear" of your ALB. 

It listens for request on a port , like : 
* Port 80 : HTTP
* Port 443: HTTPS


### What are listeners rules ?

Listener rules are like if-else conditions or you can also say filters. 

for example,
* If URL is `/products`  -> send to Products Server. 
* If URL is `/cart` -> send to Cart Server.
* If URL is `/checkout` -> send to checkout server. 

### What is a Target Group ?

A target group is simply a group of servers that do the same job. 

Example: 

* Target Group 1 --> servers for product browsing
* Target Group 2 --> servers for Cart
* Target Group 3 --> Servers for Checkout

So instead of routing to a single server, ALB routes to entire group of servers. 



