
There are two primary approaches to caching : application caching and database caching. 



Application caching requires explicit integration in the application code itself. Usually it will check if a value is in the cache , if not retrieve the value from the database, then write that value into cache 

### Application Caching : 

Caching happens within the application layer, usually in memory (RAM) , to store frequently accessed data so the app doesn't need to request it repeatedly . 

It happens in the application server , using in-memory stores like Redis, Memcached or even local memory. 

## Database caching

Caching is done inside the database engine itself to speed up queries. 

It happens inside the DB server, using DB specific caching mechanism like: 

* Query cache
* Buffer cache/ buffer pool 
* index caching 
* page caching

Database caching is built into the database engine to reduce disk I/O and speed up related queries

