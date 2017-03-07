Worker vcores	4	
Worker spindles	1
Worker RAM	15
Workload factor	2
Worker nodes	4

		Memory	vcores
OS		1,5	2
NodeManager	1	1
DataNode	1	1
Impalad		0	0
CM Agent	1	1
HBase		0	0
Solr		0	0
YARN resources	10,5	2 (Changed from -1)


YARN NM Properties				suggested	old	new	reason
yarn.nodemanager.resource.cpu-vcores		2		4	4	not loosing power
yarn.nodemanager.resource.memory-mb		10752		3852	10752	more memory is now available
YARM RM Properties				
yarn.scheduler.minimum-allocation-vcores	1			
yarn.scheduler.maximum-allocation-vcores	4			
yarn.scheduler.increment-allocation-vcores	1			
yarn.scheduler.minimum-allocation-mb		1024			
yarn.scheduler.maximum-allocation-mb		2048		4939	4939	more RAM allocaleable
yarn.scheduler.increment-allocation-mb		1024			
Task Container Settings		MIN		
mapreduce.map.memory.mb				1024	10,5	0	1GB	More Memory
mapreduce.map.java.opts.max.heap	800	MIN		
mapreduce.map.cpu.vcores		1	2		1	2	More vcores
mapreduce.reduce.memory.mb			1024			
mapreduce.reduce.java.opts.max.heap		800			
mapreduce.reduce.cpu.vcores			1			
MapReduce AM Settings				
yarn.app.mapreduce.am.resource.mb		1			
yarn.app.mapreduce.am.resource.command-opts	800			
yarn.app.mapreduce.am.resource.cpu-vcores	1			
Gateway Settings				
-D mapreduce.map.memory.mb			2048		1024	2048	more memory useable
-D mapreduce.reduce.memory.mb			4096		0	4096	more memory useable
-D mapreduce.map.java.opts.max.heap		1638,4		0	1638,4	higher heap
-D mapreduce.reduce.java.opts.max.heap		3276,8		0	3276,8	set a maximum
-D mapreduce.job.maps				2			
mapreduce.job.reduces				2		8	2	not to many jobs at the same time




What criteria affects workload factor? What does a value of 1, 2, or 4 signify?
In our case there is no influence because we changed the Value of vcores on YARN ressources to 2. In bigger environments it is for a relation between the vcores and synchrone mapreduce jobs.