#Setup

## Cloudprovider
```
AWS  
```
##Nodes
```
172.31.7.179    SK-Node1
172.31.6.8      SK-Node2
172.31.0.171    SK-Node3
172.31.9.231    SK-Node4
172.31.4.146    SK-Node5
```
##Version
```
cat /etc/redhat-release
Red Hat Enterprise Linux Server release 7.2 (Maipo)
```
##Diskspace
```
df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda2       30G  1.2G   29G   4% /
devtmpfs        7.3G     0  7.3G   0% /dev
tmpfs           7.2G     0  7.2G   0% /dev/shm
tmpfs           7.2G   17M  7.2G   1% /run
tmpfs           7.2G     0  7.2G   0% /sys/fs/cgroup
tmpfs           1.5G     0  1.5G   0% /run/user/1000
```
##repolist
```
yum repolist enabled
Loaded plugins: amazon-id, rhui-lb, search-disabled-repos
repo id                                           repo name                             status
*!epel/x86_64                                     Extra Packages for Enterprise Linux 7 11,307
!rhui-REGION-client-config-server-7/x86_64        Red Hat Update Infrastructure 2.0 Cli      4
!rhui-REGION-rhel-server-releases/7Server/x86_64  Red Hat Enterprise Linux Server 7 (RP 14,038
!rhui-REGION-rhel-server-rh-common/7Server/x86_64 Red Hat Enterprise Linux Server 7 RH     209
repolist: 25,558
```
#addin linux accounts on all nodes
```
[root@ip-172-31-7-179 ec2-user]# useradd -u 2010 neymar
[root@ip-172-31-7-179 ec2-user]# useradd -u 2016 ronaldo
[root@ip-172-31-7-179 ec2-user]# groupadd barca
[root@ip-172-31-7-179 ec2-user]# usermod -a -G barca ronaldo
[root@ip-172-31-7-179 ec2-user]# groupadd merengues
[root@ip-172-31-7-179 ec2-user]# usermod -a -G merengues neymar
[root@ip-172-31-7-179 ec2-user]# list /etc/passwd
```
##list passwd
```
cat /etc/passwd
neymar:x:2010:2010::/home/neymar:/bin/bash
ronaldo:x:2016:2016::/home/ronaldo:/bin/bash
```
##list groups
```
barca:x:2017:ronaldo
merengues:x:2018:neymar
```

