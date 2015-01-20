
# OpenFlow: enabling innovation in campus network 

@(paper)[ OpenFlow ]

**Author**: N. McKeown, G. Parulkar, T. Anderson, H. Balakrishnan, J. Rexford, L. Peterson, J. Turner, S. Shenker             
**Article Type**: review                   
**Article Source**: ACM SIGCOMM Computer Communication Review, 2008                      
**Keywords**: Ethernet Switch, virtualization, flow-based               

## OpenFlow

#### Require:
+ high-performance & low-cost
+ support board range of research
+ isolate experimental traffic from production traffic
+ consistent with vendor's closed platform

### OpenFlow Switch
**openflow switch** -> Flow Table + Secure Channel + OpenFlow Protocol

### flow-entry 

-> **action**
1. forword flow packet to a given port    
2. encapsulate and forward flow packet to a controller     
3. drop flow packet     
4. forword flow packet through switch's normal processing pipeline (key is **isolation**)     
4'.define separate sets of VLANs for experiment and production traffic      

-> **entry**
1. packet header -> define the flow     
2. action -> how the packet should be processed              
3. statistic -> flow(number of packet, bytes, time since last packet match)      

### Controller
(Type 1 switch)
add or remove flow-entries from Flow Table

*requirment*
- performance 
- reliability
- scalability
- redundancy

## Using OpenFlow
_

## Deploying OpenFlow Switch
_

## Thought

+ To understand the basic points of OpenFlow
+ Google just use the basic openflow protocol, and create a SDN implementation accoroding to their needs.



