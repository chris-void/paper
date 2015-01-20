
# NOX: Towards an os for network

@(paper)[ Controller ]

**Author**: N. Gude, T. Koponen, J. Pettit, B. Pfaff, M. Casado, N. McKeown, S. Shenker               
**Article Type**: Review                   
**Article Source**: ACM SIGCOMM Computer Communication Review, 2008                     
**Keywords**: Architecture, Management, Network, Security               

## Network OS
-> **control** & **observe** 

### major conceptual departure 
1. present programs with a *centralized programming model*
2. programs are high-level abstration

## NOX 
### Component 
-> serval *controllers* + single *network view* 

### Granularity
?? 

### Switch Abstraction
OF-> **<header: counters, actions>** 
> entry in flow-tble
	
### Operation
- **match** -> counter++ && take action
- **not match** -> forward to controller

### Scaling 伸缩性
- time scale
- consistency
### Implementation Status 
### Public Release

## Programmatic Interface

### Events
**event**     
event handlers are executed in priority

### Network View and Namespace

### Control

### Higher-level Services

### Interface & Runtime Limitation

## Thought

