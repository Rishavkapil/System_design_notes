

## How a Network Load Balancer work 

NLBs distribute traffic based on the Network conditions. For Example, if you have multiple database servers with duplicate data, the NLBs route traffic based on predetermined server IP addresses or server availability. 

The NLBs monitors the health of its registered targets and routes traffic only to the healthy targets. After a load balancer request, it selects a target from the target group for the default rule. 

It attempts to open a TCP connection to the selected target on the port specified in the listener configuration 



