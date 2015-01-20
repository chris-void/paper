## Google 
**economies of scale**     
一定科技水平下生产能力的扩大，使长期平均成本下降的趋势

1. storage
2. compute componments
3. WAN fabric -> cost efficiency, high performance, fault tolerance, manageability

+ I-scale:
+ G-scale: deployed a OpenFlow powered SDN solution 

### detail
"On this WAN fabric we built a centralized traffic engineering (TE) service. The service collects real-time utilization metrics and topology data from the underlying network and bandwidth demand from applications/services. With this data, it computes the path assignments for traffic flows and then programs the paths into the switches using OpenFlow. In the case of changing demand or network events, the service re-computes path assignments and reprograms the switches."

## Benefits of SDN:
+ Unified view of the network fabric
With SDN we get a unified view of the network, simplifying configuration, management and provisioning.

+ High utilization 
Centralized traffic engineering provides a global view of the supply and demand of network resources. Managing end-to-end paths with this global view results in high utilization of the links.

+ Faster failure handling 
Failures whether it be link, node or otherwise are handled much faster. Furthermore, the systems converge more rapidly to target optimum and the behavior is predictable.

+ Faster time to market/deployment
With SDN,better and more rigorous testing is done ahead of rollout accelerating deployment. The development is also expedited as only the features needed are developed.

+ Hitless upgrades 
The decoupling of the control plane from the forwarding/data plane enables us to perform hitless software upgrades without packet loss or capacity degradation.

+ High fidelity test environment
The entire backbone is emulated in software which not only helps in testing and verification but also in running “what-if” scenarios.

+Elastic compute 
Compute capability of network devices is no longer a limiting factor as control and management resides on external servers/controllers. Large-scale computation, path optimization in our case, is done using the latest generation of servers.


## Challenges

+ OpenFlow protocol
The OpenFlow protocol is in its in fancy and is barebones. However, as our deployment shows, it is good enough for many network applications.

+ Fault tolerant OpenFlow controllers 
To provide fault tolerance, multiple OpenFlow controllers must be provisioned. This requires handling master election and partitions between the controllers.

+ Partitioning functionality 
It is not very clear what functionality should reside in the network devices and what should reside in external controllers. Configuration of functionality resident in the network device remains an open question.


+ Flow programming 
For large networks, programming of individual flows can take a long time.
