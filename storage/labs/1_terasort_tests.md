[hdfs@ip-172-31-0-164 ~]$ hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar terasort /sebastiankramp/teragen-1G /sebastiankramp/terasort-1G
17/03/07 07:36:23 INFO terasort.TeraSort: starting
17/03/07 07:36:25 INFO input.FileInputFormat: Total input paths to process : 4
Spent 139ms computing base-splits.
Spent 2ms computing TeraScheduler splits.
Computing input splits took 142ms
Sampling 10 splits of 32
Making 8 from 100000 sampled records
Computing parititions took 6524ms
Spent 6668ms computing partitions.
17/03/07 07:36:31 INFO client.RMProxy: Connecting to ResourceManager at ec2-54-191-166-77.us-west-2.compute.amazonaws.com/172.31.0.164:8032
17/03/07 07:36:32 INFO mapreduce.JobSubmitter: number of splits:32
17/03/07 07:36:32 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1488888363816_0004
17/03/07 07:36:32 INFO impl.YarnClientImpl: Submitted application application_1488888363816_0004
17/03/07 07:36:32 INFO mapreduce.Job: The url to track the job: http://ec2-54-191-166-77.us-west-2.compute.amazonaws.com:8088/proxy/application_1488888363816_0004/
17/03/07 07:36:32 INFO mapreduce.Job: Running job: job_1488888363816_0004
17/03/07 07:36:40 INFO mapreduce.Job: Job job_1488888363816_0004 running in uber mode : false
17/03/07 07:36:40 INFO mapreduce.Job:  map 0% reduce 0%
17/03/07 07:36:49 INFO mapreduce.Job:  map 6% reduce 0%
17/03/07 07:36:50 INFO mapreduce.Job:  map 13% reduce 0%
17/03/07 07:36:51 INFO mapreduce.Job:  map 16% reduce 0%
17/03/07 07:36:52 INFO mapreduce.Job:  map 20% reduce 0%
17/03/07 07:36:53 INFO mapreduce.Job:  map 25% reduce 0%
17/03/07 07:36:57 INFO mapreduce.Job:  map 28% reduce 0%
17/03/07 07:36:58 INFO mapreduce.Job:  map 34% reduce 0%
17/03/07 07:36:59 INFO mapreduce.Job:  map 41% reduce 0%
17/03/07 07:37:01 INFO mapreduce.Job:  map 47% reduce 0%
17/03/07 07:37:05 INFO mapreduce.Job:  map 49% reduce 0%
17/03/07 07:37:06 INFO mapreduce.Job:  map 56% reduce 0%
17/03/07 07:37:08 INFO mapreduce.Job:  map 63% reduce 0%
17/03/07 07:37:09 INFO mapreduce.Job:  map 66% reduce 0%
17/03/07 07:37:10 INFO mapreduce.Job:  map 69% reduce 0%
17/03/07 07:37:11 INFO mapreduce.Job:  map 72% reduce 0%
17/03/07 07:37:14 INFO mapreduce.Job:  map 78% reduce 0%
17/03/07 07:37:16 INFO mapreduce.Job:  map 81% reduce 0%
17/03/07 07:37:17 INFO mapreduce.Job:  map 94% reduce 0%
17/03/07 07:37:18 INFO mapreduce.Job:  map 97% reduce 0%
17/03/07 07:37:20 INFO mapreduce.Job:  map 100% reduce 0%
17/03/07 07:37:30 INFO mapreduce.Job:  map 100% reduce 32%
17/03/07 07:37:31 INFO mapreduce.Job:  map 100% reduce 97%
17/03/07 07:37:32 INFO mapreduce.Job:  map 100% reduce 100%
17/03/07 07:37:33 INFO mapreduce.Job: Job job_1488888363816_0004 completed successfully
17/03/07 07:37:33 INFO mapreduce.Job: Counters: 49
        File System Counters
                FILE: Number of bytes read=439893360
                FILE: Number of bytes written=879002432
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=1000003936
                HDFS: Number of bytes written=1000000000
                HDFS: Number of read operations=120
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=16
        Job Counters
                Launched map tasks=32
                Launched reduce tasks=8
                Data-local map tasks=32
                Total time spent by all maps in occupied slots (ms)=260950
                Total time spent by all reduces in occupied slots (ms)=89204
                Total time spent by all map tasks (ms)=260950
                Total time spent by all reduce tasks (ms)=89204
                Total vcore-seconds taken by all map tasks=260950
                Total vcore-seconds taken by all reduce tasks=89204
                Total megabyte-seconds taken by all map tasks=267212800
                Total megabyte-seconds taken by all reduce tasks=91344896
        Map-Reduce Framework
                Map input records=10000000
                Map output records=10000000
                Map output bytes=1020000000
                Map output materialized bytes=434061578
                Input split bytes=3936
                Combine input records=0
                Combine output records=0
                Reduce input groups=10000000
                Reduce shuffle bytes=434061578
                Reduce input records=10000000
                Reduce output records=10000000
                Spilled Records=20000000
                Shuffled Maps =256
                Failed Shuffles=0
                Merged Map outputs=256
                GC time elapsed (ms)=3002
                CPU time spent (ms)=166170
                Physical memory (bytes) snapshot=18211594240
                Virtual memory (bytes) snapshot=63586521088
                Total committed heap usage (bytes)=21021851648
        Shuffle Errors
                BAD_ID=0
                CONNECTION=0
                IO_ERROR=0
                WRONG_LENGTH=0
                WRONG_MAP=0
                WRONG_REDUCE=0
        File Input Format Counters
                Bytes Read=1000000000
        File Output Format Counters
                Bytes Written=1000000000
17/03/07 07:37:33 INFO terasort.TeraSort: done
[hdfs@ip-172-31-0-164 ~]$
