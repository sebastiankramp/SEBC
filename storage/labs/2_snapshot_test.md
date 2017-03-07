[hdfs@ip-172-31-0-164 ~]$ hdfs dfs -createSnapshot /precious sebc-hdfs-test
Created snapshot /precious/.snapshot/sebc-hdfs-test
[hdfs@ip-172-31-0-164 ~]$ hadoop fs -ls /precious
Found 1 items
-rw-r--r--   3 hdfs supergroup     415069 2017-03-07 08:27 /precious/SEBC.zip
