
##tables are empty because they can't be recreated after kerberos is activated

```
beeline> !connect jdbc:hive2://ec2-54-187-169-81.us-west-2.compute.amazonaws.com:10000/default;principal=hive/ec2-54-187-169-81.us-west-2.compute.amazonaws.com@BASTI.LOCAL
Connecting to jdbc:hive2://ec2-54-187-169-81.us-west-2.compute.amazonaws.com:10000/default;principal=hive/ec2-54-187-169-81.us-west-2.compute.amazonaws.com@BASTI.LOCAL
Connected to: Apache Hive (version 1.1.0-cdh5.10.0)
Driver: Hive JDBC (version 1.1.0-cdh5.10.0)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://ec2-54-187-169-81.us-west-2.c> show tables;
INFO  : Compiling command(queryId=hive_20170309103838_1394e263-3ff2-4bf4-80b6-2d1c95121a63): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170309103838_1394e263-3ff2-4bf4-80b6-2d1c95121a63); Time taken: 0.644 seconds
INFO  : Executing command(queryId=hive_20170309103838_1394e263-3ff2-4bf4-80b6-2d1c95121a63): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170309103838_1394e263-3ff2-4bf4-80b6-2d1c95121a63); Time taken: 0.221 seconds
INFO  : OK
+-----------+--+
| tab_name  |
+-----------+--+
+-----------+--+
No rows selected (2.188 seconds)
0: jdbc:hive2://ec2-54-187-169-81.us-west-2.c> create role sentry_admin;
INFO  : Compiling command(queryId=hive_20170309103838_9feee8fe-2aea-46b2-be7b-e9ac24b6229e): create role sentry_admin
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170309103838_9feee8fe-2aea-46b2-be7b-e9ac24b6229e); Time taken: 0.076 seconds
INFO  : Executing command(queryId=hive_20170309103838_9feee8fe-2aea-46b2-be7b-e9ac24b6229e): create role sentry_admin
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170309103838_9feee8fe-2aea-46b2-be7b-e9ac24b6229e); Time taken: 0.489 seconds
INFO  : OK
No rows affected (0.58 seconds)
0: jdbc:hive2://ec2-54-187-169-81.us-west-2.c> GRANT ALL ON SERVER server1 TO ROLE sentry_admin;
INFO  : Compiling command(queryId=hive_20170309103939_6dc5ddf8-fbc2-47b9-b014-660deb187a17): GRANT ALL ON SERVER server1 TO ROLE sentry_admin
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170309103939_6dc5ddf8-fbc2-47b9-b014-660deb187a17); Time taken: 0.09 seconds
INFO  : Executing command(queryId=hive_20170309103939_6dc5ddf8-fbc2-47b9-b014-660deb187a17): GRANT ALL ON SERVER server1 TO ROLE sentry_admin
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170309103939_6dc5ddf8-fbc2-47b9-b014-660deb187a17); Time taken: 0.087 seconds
INFO  : OK
No rows affected (0.19 seconds)
0: jdbc:hive2://ec2-54-187-169-81.us-west-2.c> GRANT ROLE sentry_admin TO GROUP {testgroup1}
. . . . . . . . . . . . . . . . . . . . . . .> ;
Error: Error while compiling statement: FAILED: ParseException line 1:33 cannot recognize input near '{' 'testgroup1' '}' in identifier for principal spec (state=42000,code=40000)
0: jdbc:hive2://ec2-54-187-169-81.us-west-2.c> GRANT ROLE sentry_admin TO GROUP testgroup1;
INFO  : Compiling command(queryId=hive_20170309104141_3a5cfa20-e248-4169-8b5f-b3c1e0dc8fd8): GRANT ROLE sentry_admin TO GROUP testgroup1
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170309104141_3a5cfa20-e248-4169-8b5f-b3c1e0dc8fd8); Time taken: 0.066 seconds
INFO  : Executing command(queryId=hive_20170309104141_3a5cfa20-e248-4169-8b5f-b3c1e0dc8fd8): GRANT ROLE sentry_admin TO GROUP testgroup1
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170309104141_3a5cfa20-e248-4169-8b5f-b3c1e0dc8fd8); Time taken: 0.07 seconds
INFO  : OK
No rows affected (0.149 seconds)
[testuser1@ip-172-31-3-123 ec2-user]$ beeline
Beeline version 1.1.0-cdh5.10.0 by Apache Hive
beeline> !connect jdbc:hive2://ec2-54-187-169-81.us-west-2.compute.amazonaws.com:10000/default;principal=hive/ec2-54-187-169-81.us-west-2.compute.amazonaws.com@BASTI.LOCAL
scan complete in 2ms
Connecting to jdbc:hive2://ec2-54-187-169-81.us-west-2.compute.amazonaws.com:10000/default;principal=hive/ec2-54-187-169-81.us-west-2.compute.amazonaws.com@BASTI.LOCAL
Connected to: Apache Hive (version 1.1.0-cdh5.10.0)
Driver: Hive JDBC (version 1.1.0-cdh5.10.0)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://ec2-54-187-169-81.us-west-2.c> show tables;
INFO  : Compiling command(queryId=hive_20170309104747_20b91d6f-1571-4a5f-981c-57dbe68462b6): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170309104747_20b91d6f-1571-4a5f-981c-57dbe68462b6); Time taken: 0.069 seconds
INFO  : Executing command(queryId=hive_20170309104747_20b91d6f-1571-4a5f-981c-57dbe68462b6): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170309104747_20b91d6f-1571-4a5f-981c-57dbe68462b6); Time taken: 0.147 seconds
INFO  : OK
+-----------+--+
| tab_name  |
+-----------+--+
+-----------+--+
No rows selected (0.311 seconds)
0: jdbc:hive2://ec2-54-187-169-81.us-west-2.c> [testuser1@ip-172-31-3-123 ec2-user]$
[testuser1@ip-172-31-3-123 ec2-user]$ exit
```

##Create Users and Groups on all machines

```
[root@ip-172-31-3-123 ec2-user]# groupadd selector
[root@ip-172-31-3-123 ec2-user]# groupadd inserters
[root@ip-172-31-3-123 ec2-user]# useradd -u 1100 -g selector george
[root@ip-172-31-3-123 ec2-user]# useradd -u 1200 -g inserters ferdinand

```

##Back on beeline

```
[root@ip-172-31-3-123 ec2-user]# beeline
Beeline version 1.1.0-cdh5.10.0 by Apache Hive
beeline> !connect jdbc:hive2://ec2-54-187-169-81.us-west-2.compute.amazonaws.com@BASTI.LOCAL:10000/default;principal=hdfs/ec2-54-191-166-77.us-west-2.compute.amazonaws.com@BASTI.LOCAL
scan complete in 1ms
Connecting to jdbc:hive2://ec2-54-187-169-81.us-west-2.compute.amazonaws.com@BASTI.LOCAL:10000/default;principal=hdfs/ec2-54-191-166-77.us-west-2.compute.amazonaws.com@BASTI.LOCAL
Could not open connection to the HS2 server. Please check the server URI and if the URI is correct, then ask the administrator to check the server status.
Error: Could not open client transport with JDBC Uri: jdbc:hive2://BASTI.LOCAL:10000/default;principal=hdfs/ec2-54-191-166-77.us-west-2.compute.amazonaws.com@BASTI.LOCAL: java.net.UnknownHostException: BASTI.LOCAL (state=08S01,code=0)
beeline> !connect jdbc:hive2://ec2-54-187-169-81.us-west-2.compute.amazonaws.com:10000/default;principal=hive/ec2-54-187-169-81.us-west-2.compute.amazonaws.com@BASTI.LOCAL
Connecting to jdbc:hive2://ec2-54-187-169-81.us-west-2.compute.amazonaws.com:10000/default;principal=hive/ec2-54-187-169-81.us-west-2.compute.amazonaws.com@BASTI.LOCAL
Connected to: Apache Hive (version 1.1.0-cdh5.10.0)
Driver: Hive JDBC (version 1.1.0-cdh5.10.0)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://ec2-54-187-169-81.us-west-2.c> CREATE ROLE reads;
INFO  : Compiling command(queryId=hive_20170309105353_e0440578-9ac0-44e6-bae2-ef9c4393626f): CREATE ROLE reads
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170309105353_e0440578-9ac0-44e6-bae2-ef9c4393626f); Time taken: 0.067 seconds
INFO  : Executing command(queryId=hive_20170309105353_e0440578-9ac0-44e6-bae2-ef9c4393626f): CREATE ROLE reads
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170309105353_e0440578-9ac0-44e6-bae2-ef9c4393626f); Time taken: 0.046 seconds
INFO  : OK
No rows affected (0.166 seconds)
0: jdbc:hive2://ec2-54-187-169-81.us-west-2.c> CREATE ROLE writes;
INFO  : Compiling command(queryId=hive_20170309105454_0a0ff8a3-fb91-480e-af23-4e8d77980d78): CREATE ROLE writes
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170309105454_0a0ff8a3-fb91-480e-af23-4e8d77980d78); Time taken: 0.055 seconds
INFO  : Executing command(queryId=hive_20170309105454_0a0ff8a3-fb91-480e-af23-4e8d77980d78): CREATE ROLE writes
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170309105454_0a0ff8a3-fb91-480e-af23-4e8d77980d78); Time taken: 0.023 seconds
INFO  : OK
No rows affected (0.091 seconds)
0: jdbc:hive2://ec2-54-187-169-81.us-west-2.c>
0: jdbc:hive2://ec2-54-187-169-81.us-west-2.c>
0: jdbc:hive2://ec2-54-187-169-81.us-west-2.c>
0: jdbc:hive2://ec2-54-187-169-81.us-west-2.c>
0: jdbc:hive2://ec2-54-187-169-81.us-west-2.c>
0: jdbc:hive2://ec2-54-187-169-81.us-west-2.c> create database sample07;
INFO  : Compiling command(queryId=hive_20170309105454_487c28e5-e2cc-40fd-ad34-48e556237d9a): create database sample07
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170309105454_487c28e5-e2cc-40fd-ad34-48e556237d9a); Time taken: 0.107 seconds
INFO  : Executing command(queryId=hive_20170309105454_487c28e5-e2cc-40fd-ad34-48e556237d9a): create database sample07
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170309105454_487c28e5-e2cc-40fd-ad34-48e556237d9a); Time taken: 0.08 seconds
INFO  : OK
No rows affected (0.2 seconds)
0: jdbc:hive2://ec2-54-187-169-81.us-west-2.c> GRANT SELECT ON DATABASE default TO ROLE reads;
INFO  : Compiling command(queryId=hive_20170309105555_671d1041-ecbf-4ce9-8dd9-9ff7208fd62e): GRANT SELECT ON DATABASE default TO ROLE reads
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170309105555_671d1041-ecbf-4ce9-8dd9-9ff7208fd62e); Time taken: 0.056 seconds
INFO  : Executing command(queryId=hive_20170309105555_671d1041-ecbf-4ce9-8dd9-9ff7208fd62e): GRANT SELECT ON DATABASE default TO ROLE reads
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170309105555_671d1041-ecbf-4ce9-8dd9-9ff7208fd62e); Time taken: 0.036 seconds
INFO  : OK
No rows affected (0.104 seconds)
0: jdbc:hive2://ec2-54-187-169-81.us-west-2.c> GRANT ROLE reads TO GROUP selector;
INFO  : Compiling command(queryId=hive_20170309105555_74774def-0e07-470a-8821-d425b4aaee76): GRANT ROLE reads TO GROUP selector
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170309105555_74774def-0e07-470a-8821-d425b4aaee76); Time taken: 0.057 seconds
INFO  : Executing command(queryId=hive_20170309105555_74774def-0e07-470a-8821-d425b4aaee76): GRANT ROLE reads TO GROUP selector
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170309105555_74774def-0e07-470a-8821-d425b4aaee76); Time taken: 0.025 seconds
INFO  : OK
No rows affected (0.096 seconds)
0: jdbc:hive2://ec2-54-187-169-81.us-west-2.c> REVOKE ALL ON DATABASE default FROM ROLE writes;
INFO  : Compiling command(queryId=hive_20170309105555_32d20376-3acb-4553-9371-9a07c8224048): REVOKE ALL ON DATABASE default FROM ROLE writes
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170309105555_32d20376-3acb-4553-9371-9a07c8224048); Time taken: 0.056 seconds
INFO  : Executing command(queryId=hive_20170309105555_32d20376-3acb-4553-9371-9a07c8224048): REVOKE ALL ON DATABASE default FROM ROLE writes
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170309105555_32d20376-3acb-4553-9371-9a07c8224048); Time taken: 0.073 seconds
INFO  : OK
No rows affected (0.142 seconds)
0: jdbc:hive2://ec2-54-187-169-81.us-west-2.c> GRANT SELECT ON default.sample_07 TO ROLE writes;
INFO  : Compiling command(queryId=hive_20170309105656_45e47d82-0ee7-4120-b5c4-f1b2c6f754d8): GRANT SELECT ON default.sample_07 TO ROLE writes
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170309105656_45e47d82-0ee7-4120-b5c4-f1b2c6f754d8); Time taken: 0.058 seconds
INFO  : Executing command(queryId=hive_20170309105656_45e47d82-0ee7-4120-b5c4-f1b2c6f754d8): GRANT SELECT ON default.sample_07 TO ROLE writes
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170309105656_45e47d82-0ee7-4120-b5c4-f1b2c6f754d8); Time taken: 0.054 seconds
INFO  : OK
No rows affected (0.126 seconds)
0: jdbc:hive2://ec2-54-187-169-81.us-west-2.c> GRANT ROLE writes TO GROUP inserters;
INFO  : Compiling command(queryId=hive_20170309105656_4596b1c8-7a2f-4c0b-9b38-e1fe60ccba8a): GRANT ROLE writes TO GROUP inserters
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170309105656_4596b1c8-7a2f-4c0b-9b38-e1fe60ccba8a); Time taken: 0.054 seconds
INFO  : Executing command(queryId=hive_20170309105656_4596b1c8-7a2f-4c0b-9b38-e1fe60ccba8a): GRANT ROLE writes TO GROUP inserters
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170309105656_4596b1c8-7a2f-4c0b-9b38-e1fe60ccba8a); Time taken: 0.025 seconds
INFO  : OK
No rows affected (0.093 seconds)
0: jdbc:hive2://ec2-54-187-169-81.us-west-2.c> [root@ip-172-31-3-123 ec2-user]# ^C
[root@ip-172-31-3-123 ec2-user]#
[root@ip-172-31-3-123 ec2-user]# kinit george
Password for george@BASTI.LOCAL:
[root@ip-172-31-3-123 ec2-user]# klist
Ticket cache: FILE:/tmp/krb5cc_0
Default principal: george@BASTI.LOCAL

Valid starting       Expires              Service principal
03/09/2017 10:56:24  03/10/2017 10:56:24  krbtgt/BASTI.LOCAL@BASTI.LOCAL
        renew until 03/16/2017 11:56:24
[root@ip-172-31-3-123 ec2-user]# beeline
Beeline version 1.1.0-cdh5.10.0 by Apache Hive
beeline> !connect jdbc:hive2://ec2-54-187-169-81.us-west-2.compute.amazonaws.com:10000/default;principal=george@BASTI.LOCAL
scan complete in 2ms
Connecting to jdbc:hive2://ec2-54-187-169-81.us-west-2.compute.amazonaws.com:10000/default;principal=george@BASTI.LOCAL
Kerberos principal should have 3 parts: george@BASTI.LOCAL
0: jdbc:hive2://ec2-54-187-169-81.us-west-2.c (closed)> show tables;
Kerberos principal should have 3 parts: george@BASTI.LOCAL
Kerberos principal should have 3 parts: george@BASTI.LOCAL
[root@ip-172-31-3-123 ec2-user]# beeline
Beeline version 1.1.0-cdh5.10.0 by Apache Hive
beeline> !connect jdbc:hive2://ec2-54-187-169-81.us-west-2.compute.amazonaws.com:10000/default;principal=george@BASTI.LOCAL
```