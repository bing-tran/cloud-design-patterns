The pattern design to allow the system to continue to function and meet service level agreements, even when an increase in demand places and extreme load on resoursecs.

# Context and Problem
	- The load on a cloud application typically varies over time based on the number of active users or the type of activities they are performing.  
	- If processing requirements of the system exeed the capacity of the resources that are available, it'll suffer from poor performance and can even fail. If the system has to meet an agreed level of service, such failure could be uncacceptable.  

# Solution
	Serveral throtting strategies:  
	- Rejecting requests from an individual user who's already accessed system APIs more than n times per second over a given period of time. This requires the system to meter the use of resources for each tenant or user running an application (Service Metering).  
	- Disabling or degrading the functionality of selected nonessential services so that essential services can run unimpreded with sufficient resources. For example, streaming video output applications switch to a lower revolution.  
	- Use queue-based load leveling pattern
	- Defering operations being performed on behalf of lower priority applications or tenants.