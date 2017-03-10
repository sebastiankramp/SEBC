#install krb
```
[root@sk-node2 cloudera-scm-server]# yum install krb5-server krb5-libs
Loaded plugins: amazon-id, rhui-lb, search-disabled-repos
Package krb5-libs-1.14.1-27.el7_3.x86_64 already installed and latest version
Resolving Dependencies
--> Running transaction check
---> Package krb5-server.x86_64 0:1.14.1-27.el7_3 will be installed
--> Processing Dependency: /usr/share/dict/words for package: krb5-server-1.14.1-27.el7_3.x86_64
--> Processing Dependency: libverto-module-base for package: krb5-server-1.14.1-27.el7_3.x86_64
--> Running transaction check
---> Package libverto-libevent.x86_64 0:0.2.5-4.el7 will be installed
--> Processing Dependency: libevent-2.0.so.5()(64bit) for package: libverto-libevent-0.2.5-4.el7.x86_64
---> Package words.noarch 0:3.0-22.el7 will be installed
--> Running transaction check
---> Package libevent.x86_64 0:2.0.21-4.el7 will be installed
--> Finished Dependency Resolution

Dependencies Resolved

================================================================================
 Package          Arch   Version         Repository                        Size
================================================================================
Installing:
 krb5-server      x86_64 1.14.1-27.el7_3 rhui-REGION-rhel-server-releases 977 k
Installing for dependencies:
 libevent         x86_64 2.0.21-4.el7    rhui-REGION-rhel-server-releases 214 k
 libverto-libevent
                  x86_64 0.2.5-4.el7     rhui-REGION-rhel-server-releases 8.9 k
 words            noarch 3.0-22.el7      rhui-REGION-rhel-server-releases 1.4 M

Transaction Summary
================================================================================
Install  1 Package (+3 Dependent packages)

Total download size: 2.5 M
Installed size: 6.7 M
Is this ok [y/d/N]: y
Downloading packages:
(1/4): libverto-libevent-0.2.5-4.el7.x86_64.rpm            | 8.9 kB   00:00
(2/4): krb5-server-1.14.1-27.el7_3.x86_64.rpm              | 977 kB   00:00
(3/4): libevent-2.0.21-4.el7.x86_64.rpm                    | 214 kB   00:00
(4/4): words-3.0-22.el7.noarch.rpm                         | 1.4 MB   00:00
--------------------------------------------------------------------------------
Total                                              7.1 MB/s | 2.5 MB  00:00
Running transaction check
Running transaction test
Transaction test succeeded
Running transaction
  Installing : words-3.0-22.el7.noarch                                      1/4
  Installing : libevent-2.0.21-4.el7.x86_64                                 2/4
  Installing : libverto-libevent-0.2.5-4.el7.x86_64                         3/4
  Installing : krb5-server-1.14.1-27.el7_3.x86_64                           4/4
  Verifying  : libverto-libevent-0.2.5-4.el7.x86_64                         1/4
  Verifying  : libevent-2.0.21-4.el7.x86_64                                 2/4
  Verifying  : words-3.0-22.el7.noarch                                      3/4
  Verifying  : krb5-server-1.14.1-27.el7_3.x86_64                           4/4

Installed:
  krb5-server.x86_64 0:1.14.1-27.el7_3

Dependency Installed:
  libevent.x86_64 0:2.0.21-4.el7     libverto-libevent.x86_64 0:0.2.5-4.el7
  words.noarch 0:3.0-22.el7

Complete!
[root@sk-node2 cloudera-scm-server]#
```