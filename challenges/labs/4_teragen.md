#teragen
##call 
```bash
hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar teragen -D dfs.block.size=16777216 -D mapred.map.tasks=4 65536000 /user/neymar/tgen640
```
##output
```
[root@ip-172-31-0-171 ec2-user]# su hdfs
[hdfs@sk-node3 ec2-user]$ hadoop fs -chown neymar:hadoop /user/neymar
[hdfs@sk-node3 ec2-user]$ exit
exit
[root@ip-172-31-0-171 ec2-user]# su neymar
[neymar@sk-node3 ec2-user]$ hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar teragen -D dfs.block.size=16777216 -D mapred.map.tasks=4 65536000 /user/neymar/tgen640
17/03/10 05:38:12 INFO client.RMProxy: Connecting to ResourceManager at SK-Node1/172.31.7.179:8032
17/03/10 05:38:13 INFO terasort.TeraSort: Generating 65536000 using 4
17/03/10 05:38:14 INFO mapreduce.JobSubmitter: number of splits:4
17/03/10 05:38:14 INFO Configuration.deprecation: mapred.map.tasks is deprecated. Instead, use mapreduce.job.maps
17/03/10 05:38:14 INFO Configuration.deprecation: dfs.block.size is deprecated. Instead, use dfs.blocksize
17/03/10 05:38:15 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1489140841000_0002
17/03/10 05:38:15 INFO impl.YarnClientImpl: Submitted application application_1489140841000_0002
17/03/10 05:38:15 INFO mapreduce.Job: The url to track the job: http://sk-node1:8088/proxy/application_1489140841000_0002/
17/03/10 05:38:15 INFO mapreduce.Job: Running job: job_1489140841000_0002
17/03/10 05:38:20 INFO mapreduce.Job: Job job_1489140841000_0002 running in uber mode : false
17/03/10 05:38:20 INFO mapreduce.Job:  map 0% reduce 0%
17/03/10 05:38:32 INFO mapreduce.Job:  map 3% reduce 0%
17/03/10 05:38:35 INFO mapreduce.Job:  map 7% reduce 0%
17/03/10 05:38:38 INFO mapreduce.Job:  map 8% reduce 0%
17/03/10 05:38:45 INFO mapreduce.Job:  map 10% reduce 0%
17/03/10 05:38:48 INFO mapreduce.Job:  map 15% reduce 0%
17/03/10 05:38:51 INFO mapreduce.Job:  map 18% reduce 0%
17/03/10 05:38:54 INFO mapreduce.Job:  map 20% reduce 0%
17/03/10 05:38:57 INFO mapreduce.Job:  map 22% reduce 0%
17/03/10 05:39:00 INFO mapreduce.Job:  map 23% reduce 0%
17/03/10 05:39:06 INFO mapreduce.Job:  map 24% reduce 0%
17/03/10 05:39:18 INFO mapreduce.Job:  map 25% reduce 0%
17/03/10 05:39:21 INFO mapreduce.Job:  map 26% reduce 0%
17/03/10 05:39:24 INFO mapreduce.Job:  map 27% reduce 0%
17/03/10 05:39:27 INFO mapreduce.Job:  map 28% reduce 0%
17/03/10 05:39:28 INFO mapreduce.Job:  map 29% reduce 0%
17/03/10 05:39:30 INFO mapreduce.Job:  map 30% reduce 0%
17/03/10 05:39:33 INFO mapreduce.Job:  map 31% reduce 0%
17/03/10 05:39:36 INFO mapreduce.Job:  map 32% reduce 0%
17/03/10 05:39:37 INFO mapreduce.Job:  map 33% reduce 0%
17/03/10 05:39:39 INFO mapreduce.Job:  map 34% reduce 0%
17/03/10 05:39:42 INFO mapreduce.Job:  map 35% reduce 0%
17/03/10 05:39:45 INFO mapreduce.Job:  map 36% reduce 0%
17/03/10 05:39:46 INFO mapreduce.Job:  map 37% reduce 0%
17/03/10 05:39:48 INFO mapreduce.Job:  map 38% reduce 0%
17/03/10 05:39:49 INFO mapreduce.Job:  map 39% reduce 0%
17/03/10 05:39:52 INFO mapreduce.Job:  map 40% reduce 0%
17/03/10 05:39:55 INFO mapreduce.Job:  map 41% reduce 0%
17/03/10 05:39:58 INFO mapreduce.Job:  map 42% reduce 0%
17/03/10 05:40:00 INFO mapreduce.Job:  map 44% reduce 0%
17/03/10 05:40:01 INFO mapreduce.Job:  map 45% reduce 0%
17/03/10 05:40:04 INFO mapreduce.Job:  map 46% reduce 0%
17/03/10 05:40:06 INFO mapreduce.Job:  map 47% reduce 0%
17/03/10 05:40:09 INFO mapreduce.Job:  map 48% reduce 0%
17/03/10 05:40:12 INFO mapreduce.Job:  map 49% reduce 0%
17/03/10 05:40:15 INFO mapreduce.Job:  map 50% reduce 0%
17/03/10 05:40:19 INFO mapreduce.Job:  map 51% reduce 0%
17/03/10 05:40:21 INFO mapreduce.Job:  map 52% reduce 0%
17/03/10 05:40:24 INFO mapreduce.Job:  map 53% reduce 0%
17/03/10 05:40:25 INFO mapreduce.Job:  map 54% reduce 0%
17/03/10 05:40:28 INFO mapreduce.Job:  map 55% reduce 0%
17/03/10 05:40:31 INFO mapreduce.Job:  map 56% reduce 0%
17/03/10 05:40:34 INFO mapreduce.Job:  map 57% reduce 0%
17/03/10 05:40:37 INFO mapreduce.Job:  map 58% reduce 0%
17/03/10 05:40:39 INFO mapreduce.Job:  map 59% reduce 0%
17/03/10 05:40:42 INFO mapreduce.Job:  map 60% reduce 0%
17/03/10 05:40:43 INFO mapreduce.Job:  map 61% reduce 0%
17/03/10 05:40:45 INFO mapreduce.Job:  map 62% reduce 0%
17/03/10 05:40:46 INFO mapreduce.Job:  map 63% reduce 0%
17/03/10 05:40:49 INFO mapreduce.Job:  map 64% reduce 0%
17/03/10 05:40:52 INFO mapreduce.Job:  map 65% reduce 0%
17/03/10 05:40:54 INFO mapreduce.Job:  map 66% reduce 0%
17/03/10 05:40:57 INFO mapreduce.Job:  map 67% reduce 0%
17/03/10 05:40:58 INFO mapreduce.Job:  map 68% reduce 0%
17/03/10 05:41:01 INFO mapreduce.Job:  map 69% reduce 0%
17/03/10 05:41:04 INFO mapreduce.Job:  map 70% reduce 0%
17/03/10 05:41:06 INFO mapreduce.Job:  map 71% reduce 0%
17/03/10 05:41:07 INFO mapreduce.Job:  map 72% reduce 0%
17/03/10 05:41:09 INFO mapreduce.Job:  map 73% reduce 0%
17/03/10 05:41:12 INFO mapreduce.Job:  map 74% reduce 0%
17/03/10 05:41:13 INFO mapreduce.Job:  map 75% reduce 0%
17/03/10 05:41:16 INFO mapreduce.Job:  map 76% reduce 0%
17/03/10 05:41:18 INFO mapreduce.Job:  map 77% reduce 0%
17/03/10 05:41:19 INFO mapreduce.Job:  map 78% reduce 0%
17/03/10 05:41:21 INFO mapreduce.Job:  map 79% reduce 0%
17/03/10 05:41:22 INFO mapreduce.Job:  map 80% reduce 0%
17/03/10 05:41:25 INFO mapreduce.Job:  map 81% reduce 0%
17/03/10 05:41:33 INFO mapreduce.Job:  map 82% reduce 0%
17/03/10 05:41:36 INFO mapreduce.Job:  map 83% reduce 0%
17/03/10 05:41:45 INFO mapreduce.Job:  map 84% reduce 0%
17/03/10 05:41:55 INFO mapreduce.Job:  map 85% reduce 0%
17/03/10 05:42:06 INFO mapreduce.Job:  map 86% reduce 0%
17/03/10 05:42:07 INFO mapreduce.Job:  map 87% reduce 0%
17/03/10 05:42:18 INFO mapreduce.Job:  map 88% reduce 0%
17/03/10 05:42:19 INFO mapreduce.Job:  map 90% reduce 0%
17/03/10 05:42:21 INFO mapreduce.Job:  map 91% reduce 0%
17/03/10 05:42:22 INFO mapreduce.Job:  map 92% reduce 0%
17/03/10 05:42:25 INFO mapreduce.Job:  map 93% reduce 0%
17/03/10 05:42:30 INFO mapreduce.Job:  map 94% reduce 0%
17/03/10 05:42:32 INFO mapreduce.Job:  map 100% reduce 0%
17/03/10 05:42:32 INFO mapreduce.Job: Job job_1489140841000_0002 completed successfully
17/03/10 05:42:32 INFO mapreduce.Job: Counters: 31
        File System Counters
                FILE: Number of bytes read=0
                FILE: Number of bytes written=489304
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=339
                HDFS: Number of bytes written=6553600000
                HDFS: Number of read operations=16
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=8
        Job Counters
                Launched map tasks=4
                Other local map tasks=4
                Total time spent by all maps in occupied slots (ms)=975908
                Total time spent by all reduces in occupied slots (ms)=0
                Total time spent by all map tasks (ms)=975908
                Total vcore-seconds taken by all map tasks=975908
                Total megabyte-seconds taken by all map tasks=999329792
        Map-Reduce Framework
                Map input records=65536000
                Map output records=65536000
                Input split bytes=339
                Spilled Records=0
                Failed Shuffles=0
                Merged Map outputs=0
                GC time elapsed (ms)=1165
                CPU time spent (ms)=108360
                Physical memory (bytes) snapshot=749441024
                Virtual memory (bytes) snapshot=6318886912
                Total committed heap usage (bytes)=925892608
        org.apache.hadoop.examples.terasort.TeraGen$Counters
                CHECKSUM=140750829423462787
        File Input Format Counters
                Bytes Read=0
        File Output Format Counters
                Bytes Written=6553600000
[neymar@sk-node3 ec2-user]$

```
##folder
```
[hdfs@sk-node2 cloudera-scm-server]$ hdfs dfs -ls /user/neymar/tgen640
Found 5 items
-rw-r--r--   3 neymar hadoop          0 2017-03-10 05:42 /user/neymar/tgen640/_SUCCESS
-rw-r--r--   3 neymar hadoop 1638400000 2017-03-10 05:42 /user/neymar/tgen640/part-m-00000
-rw-r--r--   3 neymar hadoop 1638400000 2017-03-10 05:42 /user/neymar/tgen640/part-m-00001
-rw-r--r--   3 neymar hadoop 1638400000 2017-03-10 05:42 /user/neymar/tgen640/part-m-00002
-rw-r--r--   3 neymar hadoop 1638400000 2017-03-10 05:42 /user/neymar/tgen640/part-m-00003

```