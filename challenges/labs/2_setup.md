#my setup
```
[root@ip-172-31-6-8 ec2-user]# yum install cloudera-manager-daemons cloudera-manager-server
Loaded plugins: amazon-id, rhui-lb, search-disabled-repos
Resolving Dependencies
--> Running transaction check
---> Package cloudera-manager-daemons.x86_64 0:5.9.1-1.cm591.p0.8.el5 will be installed
---> Package cloudera-manager-server.x86_64 0:5.9.1-1.cm591.p0.8.el5 will be installed
--> Finished Dependency Resolution

Dependencies Resolved

==============================================================================================
 Package                     Arch      Version                      Repository           Size
==============================================================================================
Installing:
 cloudera-manager-daemons    x86_64    5.9.1-1.cm591.p0.8.el5       cloudera-manager    547 M
 cloudera-manager-server     x86_64    5.9.1-1.cm591.p0.8.el5       cloudera-manager    8.0 k

Transaction Summary
==============================================================================================
Install  2 Packages

Total download size: 547 M
Installed size: 673 M
Is this ok [y/d/N]: y
Downloading packages:
(1/2): cloudera-manager-server-5.9.1-1.cm591.p0.8.el5.x86_64.rpm       | 8.0 kB  00:00:00
(2/2): cloudera-manager-daemons-5.9.1-1.cm591.p0.8.el5.x86_64.rpm      | 547 MB  00:00:12
----------------------------------------------------------------------------------------------
Total                                                          44 MB/s | 547 MB  00:00:12
Running transaction check
Running transaction test
Transaction test succeeded
Running transaction
  Installing : cloudera-manager-daemons-5.9.1-1.cm591.p0.8.el5.x86_64                     1/2
  Installing : cloudera-manager-server-5.9.1-1.cm591.p0.8.el5.x86_64                      2/2
  Verifying  : cloudera-manager-daemons-5.9.1-1.cm591.p0.8.el5.x86_64                     1/2
  Verifying  : cloudera-manager-server-5.9.1-1.cm591.p0.8.el5.x86_64                      2/2

Installed:
  cloudera-manager-daemons.x86_64 0:5.9.1-1.cm591.p0.8.el5
  cloudera-manager-server.x86_64 0:5.9.1-1.cm591.p0.8.el5

Complete!
[root@ip-172-31-6-8 ec2-user]#

```