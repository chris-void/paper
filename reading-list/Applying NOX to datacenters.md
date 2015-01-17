# Applying NOX to datacenters

@(paper)[Cloud]

**Author**: A. Tavakoli, M. Casado, T. Koponen, S. Shenker
**Article Type**: conference
**Article Source**: the 2014 ACM conference on SIGCOMM
**Keywords**: SDN BGP  IXP


## MAIN

- **enterprise network:**  grow organically
- ****

### Dataenter
+ **bare-metal** datacenter:
+ ****
+ ****

### NOX
Important feature: 
+ **NOX provides complete visiablity of the network topology** -> minimize the flow latency     
use topology info to pre-load forward tables in the switches      
       
+ **NOX can operate in pro-active or re-actice** -> allow the controller to make decisions on a flow-by-flow basis, taking QoS && load condition into count     
switches send the first packet from each new flow to a controller, the controller installs the appropriate flow entries along the desired route after consulting the its topology info     

## Thought 
论述了Datacenter中对于网络的要求是什么，然后说明了为什么NOX的应用可以support **small forwarding tables, broadcast, isolation, local independence, load balancing**，还证明了NOX可以提供QoS, middlebox traversal, network visiablity, finer-grained control等等      



### Reference
[1]     
[2]     
[3] rack < (ToR switch) *connect2* internal hierarchical network < (Aggregation switches & Core routers)        
[4] 逻辑控制 -> logically centralized view of the network, **general management plane**          
[5]          
[6]           
[7] NOX -> 抽象了 user、拓扑服务、通过在switch forwarding table维持flow entries进行网络控制, access to **network observation, control promitives**, flexible and scalable platform             
[8]            
[9]           
[10]            
