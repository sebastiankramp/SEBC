[root@ip-172-31-7-179 ec2-user]# yum install mysql-server
Loaded plugins: amazon-id, rhui-lb, search-disabled-repos
mysql-connectors-community                                                                                                                                                                              | 2.5 kB  00:00:00
mysql-tools-community                                                                                                                                                                                   | 2.5 kB  00:00:00
mysql56-community                                                                                                                                                                                       | 2.5 kB  00:00:00
(1/3): mysql-connectors-community/x86_64/primary_db                                                                                                                                                     |  13 kB  00:00:00
(2/3): mysql-tools-community/x86_64/primary_db                                                                                                                                                          |  32 kB  00:00:00
(3/3): mysql56-community/x86_64/primary_db                                                                                                                                                              | 159 kB  00:00:00
Resolving Dependencies
--> Running transaction check
---> Package mysql-community-server.x86_64 0:5.6.35-2.el7 will be installed
--> Processing Dependency: mysql-community-common(x86-64) = 5.6.35-2.el7 for package: mysql-community-server-5.6.35-2.el7.x86_64
--> Processing Dependency: mysql-community-client(x86-64) >= 5.6.10 for package: mysql-community-server-5.6.35-2.el7.x86_64
--> Processing Dependency: perl(warnings) for package: mysql-community-server-5.6.35-2.el7.x86_64
--> Processing Dependency: perl(strict) for package: mysql-community-server-5.6.35-2.el7.x86_64
--> Processing Dependency: perl(if) for package: mysql-community-server-5.6.35-2.el7.x86_64
--> Processing Dependency: perl(Sys::Hostname) for package: mysql-community-server-5.6.35-2.el7.x86_64
--> Processing Dependency: perl(POSIX) for package: mysql-community-server-5.6.35-2.el7.x86_64
--> Processing Dependency: perl(Getopt::Long) for package: mysql-community-server-5.6.35-2.el7.x86_64
--> Processing Dependency: perl(File::Temp) for package: mysql-community-server-5.6.35-2.el7.x86_64
--> Processing Dependency: perl(File::Spec) for package: mysql-community-server-5.6.35-2.el7.x86_64
--> Processing Dependency: perl(File::Path) for package: mysql-community-server-5.6.35-2.el7.x86_64
--> Processing Dependency: perl(File::Copy) for package: mysql-community-server-5.6.35-2.el7.x86_64
--> Processing Dependency: perl(File::Basename) for package: mysql-community-server-5.6.35-2.el7.x86_64
--> Processing Dependency: perl(Fcntl) for package: mysql-community-server-5.6.35-2.el7.x86_64
--> Processing Dependency: perl(Data::Dumper) for package: mysql-community-server-5.6.35-2.el7.x86_64
--> Processing Dependency: perl(DBI) for package: mysql-community-server-5.6.35-2.el7.x86_64
--> Processing Dependency: libaio.so.1(LIBAIO_0.4)(64bit) for package: mysql-community-server-5.6.35-2.el7.x86_64
--> Processing Dependency: libaio.so.1(LIBAIO_0.1)(64bit) for package: mysql-community-server-5.6.35-2.el7.x86_64
--> Processing Dependency: /usr/bin/perl for package: mysql-community-server-5.6.35-2.el7.x86_64
--> Processing Dependency: libaio.so.1()(64bit) for package: mysql-community-server-5.6.35-2.el7.x86_64
--> Running transaction check
---> Package libaio.x86_64 0:0.3.109-13.el7 will be installed
---> Package mysql-community-client.x86_64 0:5.6.35-2.el7 will be installed
--> Processing Dependency: mysql-community-libs(x86-64) >= 5.6.10 for package: mysql-community-client-5.6.35-2.el7.x86_64
--> Processing Dependency: perl(Exporter) for package: mysql-community-client-5.6.35-2.el7.x86_64
---> Package mysql-community-common.x86_64 0:5.6.35-2.el7 will be installed
---> Package perl.x86_64 4:5.16.3-291.el7 will be installed
--> Processing Dependency: perl-libs = 4:5.16.3-291.el7 for package: 4:perl-5.16.3-291.el7.x86_64
--> Processing Dependency: perl(Scalar::Util) >= 1.10 for package: 4:perl-5.16.3-291.el7.x86_64
--> Processing Dependency: perl(Socket) >= 1.3 for package: 4:perl-5.16.3-291.el7.x86_64
--> Processing Dependency: perl(Carp) for package: 4:perl-5.16.3-291.el7.x86_64
--> Processing Dependency: perl(Filter::Util::Call) for package: 4:perl-5.16.3-291.el7.x86_64
--> Processing Dependency: perl(Pod::Simple::Search) for package: 4:perl-5.16.3-291.el7.x86_64
--> Processing Dependency: perl(Pod::Simple::XHTML) for package: 4:perl-5.16.3-291.el7.x86_64
--> Processing Dependency: perl(Scalar::Util) for package: 4:perl-5.16.3-291.el7.x86_64
--> Processing Dependency: perl(Socket) for package: 4:perl-5.16.3-291.el7.x86_64
--> Processing Dependency: perl(Storable) for package: 4:perl-5.16.3-291.el7.x86_64
--> Processing Dependency: perl(Time::HiRes) for package: 4:perl-5.16.3-291.el7.x86_64
--> Processing Dependency: perl(Time::Local) for package: 4:perl-5.16.3-291.el7.x86_64
--> Processing Dependency: perl(constant) for package: 4:perl-5.16.3-291.el7.x86_64
--> Processing Dependency: perl(threads) for package: 4:perl-5.16.3-291.el7.x86_64
--> Processing Dependency: perl(threads::shared) for package: 4:perl-5.16.3-291.el7.x86_64
--> Processing Dependency: perl-libs for package: 4:perl-5.16.3-291.el7.x86_64
--> Processing Dependency: perl-macros for package: 4:perl-5.16.3-291.el7.x86_64
--> Processing Dependency: libperl.so()(64bit) for package: 4:perl-5.16.3-291.el7.x86_64
---> Package perl-DBI.x86_64 0:1.627-4.el7 will be installed
--> Processing Dependency: perl(RPC::PlClient) >= 0.2000 for package: perl-DBI-1.627-4.el7.x86_64
--> Processing Dependency: perl(RPC::PlServer) >= 0.2001 for package: perl-DBI-1.627-4.el7.x86_64
---> Package perl-Data-Dumper.x86_64 0:2.145-3.el7 will be installed
---> Package perl-File-Path.noarch 0:2.09-2.el7 will be installed
---> Package perl-File-Temp.noarch 0:0.23.01-3.el7 will be installed
---> Package perl-Getopt-Long.noarch 0:2.40-2.el7 will be installed
--> Processing Dependency: perl(Pod::Usage) >= 1.14 for package: perl-Getopt-Long-2.40-2.el7.noarch
--> Processing Dependency: perl(Text::ParseWords) for package: perl-Getopt-Long-2.40-2.el7.noarch
---> Package perl-PathTools.x86_64 0:3.40-5.el7 will be installed
--> Running transaction check
---> Package mariadb-libs.x86_64 1:5.5.44-2.el7 will be obsoleted
---> Package mysql-community-libs.x86_64 0:5.6.35-2.el7 will be obsoleting
---> Package perl-Carp.noarch 0:1.26-244.el7 will be installed
---> Package perl-Exporter.noarch 0:5.68-3.el7 will be installed
---> Package perl-Filter.x86_64 0:1.49-3.el7 will be installed
---> Package perl-PlRPC.noarch 0:0.2020-14.el7 will be installed
--> Processing Dependency: perl(Net::Daemon) >= 0.13 for package: perl-PlRPC-0.2020-14.el7.noarch
--> Processing Dependency: perl(Compress::Zlib) for package: perl-PlRPC-0.2020-14.el7.noarch
--> Processing Dependency: perl(Net::Daemon::Log) for package: perl-PlRPC-0.2020-14.el7.noarch
--> Processing Dependency: perl(Net::Daemon::Test) for package: perl-PlRPC-0.2020-14.el7.noarch
---> Package perl-Pod-Simple.noarch 1:3.28-4.el7 will be installed
--> Processing Dependency: perl(Pod::Escapes) >= 1.04 for package: 1:perl-Pod-Simple-3.28-4.el7.noarch
--> Processing Dependency: perl(Encode) for package: 1:perl-Pod-Simple-3.28-4.el7.noarch
---> Package perl-Pod-Usage.noarch 0:1.63-3.el7 will be installed
--> Processing Dependency: perl(Pod::Text) >= 3.15 for package: perl-Pod-Usage-1.63-3.el7.noarch
--> Processing Dependency: perl-Pod-Perldoc for package: perl-Pod-Usage-1.63-3.el7.noarch
---> Package perl-Scalar-List-Utils.x86_64 0:1.27-248.el7 will be installed
---> Package perl-Socket.x86_64 0:2.010-4.el7 will be installed
---> Package perl-Storable.x86_64 0:2.45-3.el7 will be installed
---> Package perl-Text-ParseWords.noarch 0:3.29-4.el7 will be installed
---> Package perl-Time-HiRes.x86_64 4:1.9725-3.el7 will be installed
---> Package perl-Time-Local.noarch 0:1.2300-2.el7 will be installed
---> Package perl-constant.noarch 0:1.27-2.el7 will be installed
---> Package perl-libs.x86_64 4:5.16.3-291.el7 will be installed
---> Package perl-macros.x86_64 4:5.16.3-291.el7 will be installed
---> Package perl-threads.x86_64 0:1.87-4.el7 will be installed
---> Package perl-threads-shared.x86_64 0:1.43-6.el7 will be installed
--> Running transaction check
---> Package perl-Encode.x86_64 0:2.51-7.el7 will be installed
---> Package perl-IO-Compress.noarch 0:2.061-2.el7 will be installed
--> Processing Dependency: perl(Compress::Raw::Bzip2) >= 2.061 for package: perl-IO-Compress-2.061-2.el7.noarch
--> Processing Dependency: perl(Compress::Raw::Zlib) >= 2.061 for package: perl-IO-Compress-2.061-2.el7.noarch
---> Package perl-Net-Daemon.noarch 0:0.48-5.el7 will be installed
---> Package perl-Pod-Escapes.noarch 1:1.04-291.el7 will be installed
---> Package perl-Pod-Perldoc.noarch 0:3.20-4.el7 will be installed
--> Processing Dependency: perl(HTTP::Tiny) for package: perl-Pod-Perldoc-3.20-4.el7.noarch
--> Processing Dependency: perl(parent) for package: perl-Pod-Perldoc-3.20-4.el7.noarch
---> Package perl-podlators.noarch 0:2.5.1-3.el7 will be installed
--> Running transaction check
---> Package perl-Compress-Raw-Bzip2.x86_64 0:2.061-3.el7 will be installed
---> Package perl-Compress-Raw-Zlib.x86_64 1:2.061-4.el7 will be installed
---> Package perl-HTTP-Tiny.noarch 0:0.033-3.el7 will be installed
---> Package perl-parent.noarch 1:0.225-244.el7 will be installed
--> Finished Dependency Resolution

Dependencies Resolved

===============================================================================================================================================================================================================================
 Package                                                  Arch                                    Version                                              Repository                                                         Size
===============================================================================================================================================================================================================================
Installing:
 mysql-community-libs                                     x86_64                                  5.6.35-2.el7                                         mysql56-community                                                 2.0 M
     replacing  mariadb-libs.x86_64 1:5.5.44-2.el7
 mysql-community-server                                   x86_64                                  5.6.35-2.el7                                         mysql56-community                                                  59 M
Installing for dependencies:
 libaio                                                   x86_64                                  0.3.109-13.el7                                       rhui-REGION-rhel-server-releases                                   24 k
 mysql-community-client                                   x86_64                                  5.6.35-2.el7                                         mysql56-community                                                  19 M
 mysql-community-common                                   x86_64                                  5.6.35-2.el7                                         mysql56-community                                                 257 k
 perl                                                     x86_64                                  4:5.16.3-291.el7                                     rhui-REGION-rhel-server-releases                                  8.0 M
 perl-Carp                                                noarch                                  1.26-244.el7                                         rhui-REGION-rhel-server-releases                                   19 k
 perl-Compress-Raw-Bzip2                                  x86_64                                  2.061-3.el7                                          rhui-REGION-rhel-server-releases                                   32 k
 perl-Compress-Raw-Zlib                                   x86_64                                  1:2.061-4.el7                                        rhui-REGION-rhel-server-releases                                   57 k
 perl-DBI                                                 x86_64                                  1.627-4.el7                                          rhui-REGION-rhel-server-releases                                  802 k
 perl-Data-Dumper                                         x86_64                                  2.145-3.el7                                          rhui-REGION-rhel-server-releases                                   47 k
 perl-Encode                                              x86_64                                  2.51-7.el7                                           rhui-REGION-rhel-server-releases                                  1.5 M
 perl-Exporter                                            noarch                                  5.68-3.el7                                           rhui-REGION-rhel-server-releases                                   28 k
 perl-File-Path                                           noarch                                  2.09-2.el7                                           rhui-REGION-rhel-server-releases                                   27 k
 perl-File-Temp                                           noarch                                  0.23.01-3.el7                                        rhui-REGION-rhel-server-releases                                   56 k
 perl-Filter                                              x86_64                                  1.49-3.el7                                           rhui-REGION-rhel-server-releases                                   76 k
 perl-Getopt-Long                                         noarch                                  2.40-2.el7                                           rhui-REGION-rhel-server-releases                                   56 k
 perl-HTTP-Tiny                                           noarch                                  0.033-3.el7                                          rhui-REGION-rhel-server-releases                                   38 k
 perl-IO-Compress                                         noarch                                  2.061-2.el7                                          rhui-REGION-rhel-server-releases                                  260 k
 perl-Net-Daemon                                          noarch                                  0.48-5.el7                                           rhui-REGION-rhel-server-releases                                   51 k
 perl-PathTools                                           x86_64                                  3.40-5.el7                                           rhui-REGION-rhel-server-releases                                   83 k
 perl-PlRPC                                               noarch                                  0.2020-14.el7                                        rhui-REGION-rhel-server-releases                                   36 k
 perl-Pod-Escapes                                         noarch                                  1:1.04-291.el7                                       rhui-REGION-rhel-server-releases                                   51 k
 perl-Pod-Perldoc                                         noarch                                  3.20-4.el7                                           rhui-REGION-rhel-server-releases                                   87 k
 perl-Pod-Simple                                          noarch                                  1:3.28-4.el7                                         rhui-REGION-rhel-server-releases                                  216 k
 perl-Pod-Usage                                           noarch                                  1.63-3.el7                                           rhui-REGION-rhel-server-releases                                   27 k
 perl-Scalar-List-Utils                                   x86_64                                  1.27-248.el7                                         rhui-REGION-rhel-server-releases                                   36 k
 perl-Socket                                              x86_64                                  2.010-4.el7                                          rhui-REGION-rhel-server-releases                                   49 k
 perl-Storable                                            x86_64                                  2.45-3.el7                                           rhui-REGION-rhel-server-releases                                   77 k
 perl-Text-ParseWords                                     noarch                                  3.29-4.el7                                           rhui-REGION-rhel-server-releases                                   14 k
 perl-Time-HiRes                                          x86_64                                  4:1.9725-3.el7                                       rhui-REGION-rhel-server-releases                                   45 k
 perl-Time-Local                                          noarch                                  1.2300-2.el7                                         rhui-REGION-rhel-server-releases                                   24 k
 perl-constant                                            noarch                                  1.27-2.el7                                           rhui-REGION-rhel-server-releases                                   19 k
 perl-libs                                                x86_64                                  4:5.16.3-291.el7                                     rhui-REGION-rhel-server-releases                                  688 k
 perl-macros                                              x86_64                                  4:5.16.3-291.el7                                     rhui-REGION-rhel-server-releases                                   43 k
 perl-parent                                              noarch                                  1:0.225-244.el7                                      rhui-REGION-rhel-server-releases                                   12 k
 perl-podlators                                           noarch                                  2.5.1-3.el7                                          rhui-REGION-rhel-server-releases                                  112 k
 perl-threads                                             x86_64                                  1.87-4.el7                                           rhui-REGION-rhel-server-releases                                   49 k
 perl-threads-shared                                      x86_64                                  1.43-6.el7                                           rhui-REGION-rhel-server-releases                                   39 k

Transaction Summary
===============================================================================================================================================================================================================================
Install  2 Packages (+37 Dependent packages)

Total download size: 93 M
Is this ok [y/d/N]: y
Downloading packages:
warning: /var/cache/yum/x86_64/7Server/mysql56-community/packages/mysql-community-common-5.6.35-2.el7.x86_64.rpm: Header V3 DSA/SHA1 Signature, key ID 5072e1f5: NOKEY
Public key for mysql-community-common-5.6.35-2.el7.x86_64.rpm is not installed
(1/39): mysql-community-common-5.6.35-2.el7.x86_64.rpm                                                                                                                                                  | 257 kB  00:00:00
(2/39): mysql-community-libs-5.6.35-2.el7.x86_64.rpm                                                                                                                                                    | 2.0 MB  00:00:00
(3/39): libaio-0.3.109-13.el7.x86_64.rpm                                                                                                                                                                |  24 kB  00:00:00
(4/39): perl-Compress-Raw-Bzip2-2.061-3.el7.x86_64.rpm                                                                                                                                                  |  32 kB  00:00:00
(5/39): mysql-community-client-5.6.35-2.el7.x86_64.rpm                                                                                                                                                  |  19 MB  00:00:00
(6/39): perl-Compress-Raw-Zlib-2.061-4.el7.x86_64.rpm                                                                                                                                                   |  57 kB  00:00:00
(7/39): perl-Carp-1.26-244.el7.noarch.rpm                                                                                                                                                               |  19 kB  00:00:00
(8/39): perl-DBI-1.627-4.el7.x86_64.rpm                                                                                                                                                                 | 802 kB  00:00:00
(9/39): perl-5.16.3-291.el7.x86_64.rpm                                                                                                                                                                  | 8.0 MB  00:00:00
(10/39): perl-Exporter-5.68-3.el7.noarch.rpm                                                                                                                                                            |  28 kB  00:00:00
(11/39): perl-Data-Dumper-2.145-3.el7.x86_64.rpm                                                                                                                                                        |  47 kB  00:00:00
(12/39): perl-File-Path-2.09-2.el7.noarch.rpm                                                                                                                                                           |  27 kB  00:00:00
(13/39): mysql-community-server-5.6.35-2.el7.x86_64.rpm                                                                                                                                                 |  59 MB  00:00:00
(14/39): perl-Encode-2.51-7.el7.x86_64.rpm                                                                                                                                                              | 1.5 MB  00:00:00
(15/39): perl-File-Temp-0.23.01-3.el7.noarch.rpm                                                                                                                                                        |  56 kB  00:00:00
(16/39): perl-Filter-1.49-3.el7.x86_64.rpm                                                                                                                                                              |  76 kB  00:00:00
(17/39): perl-Getopt-Long-2.40-2.el7.noarch.rpm                                                                                                                                                         |  56 kB  00:00:00
(18/39): perl-IO-Compress-2.061-2.el7.noarch.rpm                                                                                                                                                        | 260 kB  00:00:00
(19/39): perl-Net-Daemon-0.48-5.el7.noarch.rpm                                                                                                                                                          |  51 kB  00:00:00
(20/39): perl-HTTP-Tiny-0.033-3.el7.noarch.rpm                                                                                                                                                          |  38 kB  00:00:00
(21/39): perl-PathTools-3.40-5.el7.x86_64.rpm                                                                                                                                                           |  83 kB  00:00:00
(22/39): perl-PlRPC-0.2020-14.el7.noarch.rpm                                                                                                                                                            |  36 kB  00:00:00
(23/39): perl-Pod-Escapes-1.04-291.el7.noarch.rpm                                                                                                                                                       |  51 kB  00:00:00
(24/39): perl-Pod-Perldoc-3.20-4.el7.noarch.rpm                                                                                                                                                         |  87 kB  00:00:00
(25/39): perl-Pod-Usage-1.63-3.el7.noarch.rpm                                                                                                                                                           |  27 kB  00:00:00
(26/39): perl-Pod-Simple-3.28-4.el7.noarch.rpm                                                                                                                                                          | 216 kB  00:00:00
(27/39): perl-Scalar-List-Utils-1.27-248.el7.x86_64.rpm                                                                                                                                                 |  36 kB  00:00:00
(28/39): perl-Storable-2.45-3.el7.x86_64.rpm                                                                                                                                                            |  77 kB  00:00:00
(29/39): perl-Socket-2.010-4.el7.x86_64.rpm                                                                                                                                                             |  49 kB  00:00:00
(30/39): perl-Text-ParseWords-3.29-4.el7.noarch.rpm                                                                                                                                                     |  14 kB  00:00:00
(31/39): perl-Time-Local-1.2300-2.el7.noarch.rpm                                                                                                                                                        |  24 kB  00:00:00
(32/39): perl-Time-HiRes-1.9725-3.el7.x86_64.rpm                                                                                                                                                        |  45 kB  00:00:00
(33/39): perl-constant-1.27-2.el7.noarch.rpm                                                                                                                                                            |  19 kB  00:00:00
(34/39): perl-macros-5.16.3-291.el7.x86_64.rpm                                                                                                                                                          |  43 kB  00:00:00
(35/39): perl-parent-0.225-244.el7.noarch.rpm                                                                                                                                                           |  12 kB  00:00:00
(36/39): perl-libs-5.16.3-291.el7.x86_64.rpm                                                                                                                                                            | 688 kB  00:00:00
(37/39): perl-threads-1.87-4.el7.x86_64.rpm                                                                                                                                                             |  49 kB  00:00:00
(38/39): perl-podlators-2.5.1-3.el7.noarch.rpm                                                                                                                                                          | 112 kB  00:00:00
(39/39): perl-threads-shared-1.43-6.el7.x86_64.rpm                                                                                                                                                      |  39 kB  00:00:00
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Total                                                                                                                                                                                           50 MB/s |  93 MB  00:00:01
Retrieving key from file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql
Importing GPG key 0x5072E1F5:
 Userid     : "MySQL Release Engineering <mysql-build@oss.oracle.com>"
 Fingerprint: a4a9 4068 76fc bd3c 4567 70c8 8c71 8d3b 5072 e1f5
 Package    : mysql57-community-release-el7-9.noarch (@/mysql57-community-release-el7-9.noarch)
 From       : /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql
Is this ok [y/N]: <
Is this ok [y/N]: y
Running transaction check
Running transaction test
Transaction test succeeded
Running transaction
  Installing : mysql-community-common-5.6.35-2.el7.x86_64                                                                                                                                                                 1/40
  Installing : mysql-community-libs-5.6.35-2.el7.x86_64                                                                                                                                                                   2/40
  Installing : 1:perl-parent-0.225-244.el7.noarch                                                                                                                                                                         3/40
  Installing : perl-HTTP-Tiny-0.033-3.el7.noarch                                                                                                                                                                          4/40
  Installing : perl-podlators-2.5.1-3.el7.noarch                                                                                                                                                                          5/40
  Installing : perl-Pod-Perldoc-3.20-4.el7.noarch                                                                                                                                                                         6/40
  Installing : 1:perl-Pod-Escapes-1.04-291.el7.noarch                                                                                                                                                                     7/40
  Installing : perl-Encode-2.51-7.el7.x86_64                                                                                                                                                                              8/40
  Installing : perl-Text-ParseWords-3.29-4.el7.noarch                                                                                                                                                                     9/40
  Installing : perl-Pod-Usage-1.63-3.el7.noarch                                                                                                                                                                          10/40
  Installing : perl-Storable-2.45-3.el7.x86_64                                                                                                                                                                           11/40
  Installing : perl-Exporter-5.68-3.el7.noarch                                                                                                                                                                           12/40
  Installing : perl-constant-1.27-2.el7.noarch                                                                                                                                                                           13/40
  Installing : perl-Time-Local-1.2300-2.el7.noarch                                                                                                                                                                       14/40
  Installing : perl-Socket-2.010-4.el7.x86_64                                                                                                                                                                            15/40
  Installing : perl-Carp-1.26-244.el7.noarch                                                                                                                                                                             16/40
  Installing : 4:perl-Time-HiRes-1.9725-3.el7.x86_64                                                                                                                                                                     17/40
  Installing : perl-PathTools-3.40-5.el7.x86_64                                                                                                                                                                          18/40
  Installing : perl-Scalar-List-Utils-1.27-248.el7.x86_64                                                                                                                                                                19/40
  Installing : 4:perl-libs-5.16.3-291.el7.x86_64                                                                                                                                                                         20/40
  Installing : 4:perl-macros-5.16.3-291.el7.x86_64                                                                                                                                                                       21/40
  Installing : 1:perl-Pod-Simple-3.28-4.el7.noarch                                                                                                                                                                       22/40
  Installing : perl-File-Temp-0.23.01-3.el7.noarch                                                                                                                                                                       23/40
  Installing : perl-File-Path-2.09-2.el7.noarch                                                                                                                                                                          24/40
  Installing : perl-threads-shared-1.43-6.el7.x86_64                                                                                                                                                                     25/40
  Installing : perl-threads-1.87-4.el7.x86_64                                                                                                                                                                            26/40
  Installing : perl-Filter-1.49-3.el7.x86_64                                                                                                                                                                             27/40
  Installing : perl-Getopt-Long-2.40-2.el7.noarch                                                                                                                                                                        28/40
  Installing : 4:perl-5.16.3-291.el7.x86_64                                                                                                                                                                              29/40
  Installing : perl-Data-Dumper-2.145-3.el7.x86_64                                                                                                                                                                       30/40
  Installing : perl-Compress-Raw-Bzip2-2.061-3.el7.x86_64                                                                                                                                                                31/40
  Installing : mysql-community-client-5.6.35-2.el7.x86_64                                                                                                                                                                32/40
  Installing : perl-Net-Daemon-0.48-5.el7.noarch                                                                                                                                                                         33/40
  Installing : 1:perl-Compress-Raw-Zlib-2.061-4.el7.x86_64                                                                                                                                                               34/40
  Installing : perl-IO-Compress-2.061-2.el7.noarch                                                                                                                                                                       35/40
  Installing : perl-PlRPC-0.2020-14.el7.noarch                                                                                                                                                                           36/40
  Installing : perl-DBI-1.627-4.el7.x86_64                                                                                                                                                                               37/40
  Installing : libaio-0.3.109-13.el7.x86_64                                                                                                                                                                              38/40
  Installing : mysql-community-server-5.6.35-2.el7.x86_64                                                                                                                                                                39/40
  Erasing    : 1:mariadb-libs-5.5.44-2.el7.x86_64                                                                                                                                                                        40/40
  Verifying  : perl-HTTP-Tiny-0.033-3.el7.noarch                                                                                                                                                                          1/40
  Verifying  : perl-threads-shared-1.43-6.el7.x86_64                                                                                                                                                                      2/40
  Verifying  : perl-Storable-2.45-3.el7.x86_64                                                                                                                                                                            3/40
  Verifying  : perl-IO-Compress-2.061-2.el7.noarch                                                                                                                                                                        4/40
  Verifying  : perl-Exporter-5.68-3.el7.noarch                                                                                                                                                                            5/40
  Verifying  : perl-constant-1.27-2.el7.noarch                                                                                                                                                                            6/40
  Verifying  : perl-PathTools-3.40-5.el7.x86_64                                                                                                                                                                           7/40
  Verifying  : 1:perl-Pod-Escapes-1.04-291.el7.noarch                                                                                                                                                                     8/40
  Verifying  : perl-Compress-Raw-Bzip2-2.061-3.el7.x86_64                                                                                                                                                                 9/40
  Verifying  : mysql-community-client-5.6.35-2.el7.x86_64                                                                                                                                                                10/40
  Verifying  : 1:perl-parent-0.225-244.el7.noarch                                                                                                                                                                        11/40
  Verifying  : perl-Net-Daemon-0.48-5.el7.noarch                                                                                                                                                                         12/40
  Verifying  : mysql-community-libs-5.6.35-2.el7.x86_64                                                                                                                                                                  13/40
  Verifying  : perl-File-Temp-0.23.01-3.el7.noarch                                                                                                                                                                       14/40
  Verifying  : 1:perl-Pod-Simple-3.28-4.el7.noarch                                                                                                                                                                       15/40
  Verifying  : perl-Time-Local-1.2300-2.el7.noarch                                                                                                                                                                       16/40
  Verifying  : perl-Pod-Perldoc-3.20-4.el7.noarch                                                                                                                                                                        17/40
  Verifying  : perl-DBI-1.627-4.el7.x86_64                                                                                                                                                                               18/40
  Verifying  : libaio-0.3.109-13.el7.x86_64                                                                                                                                                                              19/40
  Verifying  : mysql-community-server-5.6.35-2.el7.x86_64                                                                                                                                                                20/40
  Verifying  : perl-Socket-2.010-4.el7.x86_64                                                                                                                                                                            21/40
  Verifying  : perl-Carp-1.26-244.el7.noarch                                                                                                                                                                             22/40
  Verifying  : perl-Data-Dumper-2.145-3.el7.x86_64                                                                                                                                                                       23/40
  Verifying  : 4:perl-Time-HiRes-1.9725-3.el7.x86_64                                                                                                                                                                     24/40
  Verifying  : perl-Scalar-List-Utils-1.27-248.el7.x86_64                                                                                                                                                                25/40
  Verifying  : 1:perl-Compress-Raw-Zlib-2.061-4.el7.x86_64                                                                                                                                                               26/40
  Verifying  : 4:perl-libs-5.16.3-291.el7.x86_64                                                                                                                                                                         27/40
  Verifying  : 4:perl-macros-5.16.3-291.el7.x86_64                                                                                                                                                                       28/40
  Verifying  : perl-Pod-Usage-1.63-3.el7.noarch                                                                                                                                                                          29/40
  Verifying  : perl-PlRPC-0.2020-14.el7.noarch                                                                                                                                                                           30/40
  Verifying  : perl-Encode-2.51-7.el7.x86_64                                                                                                                                                                             31/40
  Verifying  : perl-podlators-2.5.1-3.el7.noarch                                                                                                                                                                         32/40
  Verifying  : perl-Getopt-Long-2.40-2.el7.noarch                                                                                                                                                                        33/40
  Verifying  : perl-File-Path-2.09-2.el7.noarch                                                                                                                                                                          34/40
  Verifying  : 4:perl-5.16.3-291.el7.x86_64                                                                                                                                                                              35/40
  Verifying  : mysql-community-common-5.6.35-2.el7.x86_64                                                                                                                                                                36/40
  Verifying  : perl-threads-1.87-4.el7.x86_64                                                                                                                                                                            37/40
  Verifying  : perl-Filter-1.49-3.el7.x86_64                                                                                                                                                                             38/40
  Verifying  : perl-Text-ParseWords-3.29-4.el7.noarch                                                                                                                                                                    39/40
  Verifying  : 1:mariadb-libs-5.5.44-2.el7.x86_64                                                                                                                                                                        40/40

Installed:
  mysql-community-libs.x86_64 0:5.6.35-2.el7                                                                    mysql-community-server.x86_64 0:5.6.35-2.el7

Dependency Installed:
  libaio.x86_64 0:0.3.109-13.el7               mysql-community-client.x86_64 0:5.6.35-2.el7 mysql-community-common.x86_64 0:5.6.35-2.el7 perl.x86_64 4:5.16.3-291.el7          perl-Carp.noarch 0:1.26-244.el7
  perl-Compress-Raw-Bzip2.x86_64 0:2.061-3.el7 perl-Compress-Raw-Zlib.x86_64 1:2.061-4.el7  perl-DBI.x86_64 0:1.627-4.el7                perl-Data-Dumper.x86_64 0:2.145-3.el7 perl-Encode.x86_64 0:2.51-7.el7
  perl-Exporter.noarch 0:5.68-3.el7            perl-File-Path.noarch 0:2.09-2.el7           perl-File-Temp.noarch 0:0.23.01-3.el7        perl-Filter.x86_64 0:1.49-3.el7       perl-Getopt-Long.noarch 0:2.40-2.el7
  perl-HTTP-Tiny.noarch 0:0.033-3.el7          perl-IO-Compress.noarch 0:2.061-2.el7        perl-Net-Daemon.noarch 0:0.48-5.el7          perl-PathTools.x86_64 0:3.40-5.el7    perl-PlRPC.noarch 0:0.2020-14.el7
  perl-Pod-Escapes.noarch 1:1.04-291.el7       perl-Pod-Perldoc.noarch 0:3.20-4.el7         perl-Pod-Simple.noarch 1:3.28-4.el7          perl-Pod-Usage.noarch 0:1.63-3.el7    perl-Scalar-List-Utils.x86_64 0:1.27-248.el7
  perl-Socket.x86_64 0:2.010-4.el7             perl-Storable.x86_64 0:2.45-3.el7            perl-Text-ParseWords.noarch 0:3.29-4.el7     perl-Time-HiRes.x86_64 4:1.9725-3.el7 perl-Time-Local.noarch 0:1.2300-2.el7
  perl-constant.noarch 0:1.27-2.el7            perl-libs.x86_64 4:5.16.3-291.el7            perl-macros.x86_64 4:5.16.3-291.el7          perl-parent.noarch 1:0.225-244.el7    perl-podlators.noarch 0:2.5.1-3.el7
  perl-threads.x86_64 0:1.87-4.el7             perl-threads-shared.x86_64 0:1.43-6.el7

Replaced:
  mariadb-libs.x86_64 1:5.5.44-2.el7

Complete!
[root@ip-172-31-7-179 ec2-user]# yum install mysql
Loaded plugins: amazon-id, rhui-lb, search-disabled-repos
Package mysql-community-client-5.6.35-2.el7.x86_64 already installed and latest version
Nothing to do
[root@ip-172-31-7-179 ec2-user]# b.wget https://dev.mysql.com/get/Downloads/Connector-J/mysql-connector-java-                                                                                                                  5.1.41.tar.gz
bash: b.wget: command not found
[root@ip-172-31-7-179 ec2-user]# wget https://dev.mysql.com/get/Downloads/Connector-J/mysql-connector-java-5.                                                                                                                  1.41.tar.gz
--2017-03-10 03:28:42--  https://dev.mysql.com/get/Downloads/Connector-J/mysql-connector-java-5.1.41.tar.gz
Resolving dev.mysql.com (dev.mysql.com)... 137.254.60.11
Connecting to dev.mysql.com (dev.mysql.com)|137.254.60.11|:443... connected.
HTTP request sent, awaiting response... 302 Found
Location: https://cdn.mysql.com//Downloads/Connector-J/mysql-connector-java-5.1.41.tar.gz [following]
--2017-03-10 03:28:43--  https://cdn.mysql.com//Downloads/Connector-J/mysql-connector-java-5.1.41.tar.gz
Resolving cdn.mysql.com (cdn.mysql.com)... 104.111.217.179
Connecting to cdn.mysql.com (cdn.mysql.com)|104.111.217.179|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 3923677 (3.7M) [application/x-tar-gz]
Saving to: ‘mysql-connector-java-5.1.41.tar.gz’

100%[===================================================================>] 3,923,677   --.-K/s   in 0.06s

2017-03-10 03:28:43 (66.1 MB/s) - ‘mysql-connector-java-5.1.41.tar.gz’ saved [3923677/3923677]

[root@ip-172-31-7-179 ec2-user]# tar zxvf mysql-connector-java-5.1.41.tar.gz
mysql-connector-java-5.1.41/
mysql-connector-java-5.1.41/docs/
mysql-connector-java-5.1.41/src/
mysql-connector-java-5.1.41/src/com/
mysql-connector-java-5.1.41/src/com/mysql/
mysql-connector-java-5.1.41/src/com/mysql/fabric/
mysql-connector-java-5.1.41/src/com/mysql/fabric/hibernate/
mysql-connector-java-5.1.41/src/com/mysql/fabric/jdbc/
mysql-connector-java-5.1.41/src/com/mysql/fabric/proto/
mysql-connector-java-5.1.41/src/com/mysql/fabric/proto/xmlrpc/
mysql-connector-java-5.1.41/src/com/mysql/fabric/xmlrpc/
mysql-connector-java-5.1.41/src/com/mysql/fabric/xmlrpc/base/
mysql-connector-java-5.1.41/src/com/mysql/fabric/xmlrpc/exceptions/
mysql-connector-java-5.1.41/src/com/mysql/jdbc/
mysql-connector-java-5.1.41/src/com/mysql/jdbc/authentication/
mysql-connector-java-5.1.41/src/com/mysql/jdbc/configs/
mysql-connector-java-5.1.41/src/com/mysql/jdbc/exceptions/
mysql-connector-java-5.1.41/src/com/mysql/jdbc/exceptions/jdbc4/
mysql-connector-java-5.1.41/src/com/mysql/jdbc/integration/
mysql-connector-java-5.1.41/src/com/mysql/jdbc/integration/c3p0/
mysql-connector-java-5.1.41/src/com/mysql/jdbc/integration/jboss/
mysql-connector-java-5.1.41/src/com/mysql/jdbc/interceptors/
mysql-connector-java-5.1.41/src/com/mysql/jdbc/jdbc2/
mysql-connector-java-5.1.41/src/com/mysql/jdbc/jdbc2/optional/
mysql-connector-java-5.1.41/src/com/mysql/jdbc/jmx/
mysql-connector-java-5.1.41/src/com/mysql/jdbc/log/
mysql-connector-java-5.1.41/src/com/mysql/jdbc/profiler/
mysql-connector-java-5.1.41/src/com/mysql/jdbc/util/
mysql-connector-java-5.1.41/src/demo/
mysql-connector-java-5.1.41/src/demo/fabric/
mysql-connector-java-5.1.41/src/demo/fabric/resources/
mysql-connector-java-5.1.41/src/demo/fabric/resources/com/
mysql-connector-java-5.1.41/src/demo/fabric/resources/com/mysql/
mysql-connector-java-5.1.41/src/demo/fabric/resources/com/mysql/fabric/
mysql-connector-java-5.1.41/src/demo/fabric/resources/com/mysql/fabric/demo/
mysql-connector-java-5.1.41/src/doc/
mysql-connector-java-5.1.41/src/doc/sources/
mysql-connector-java-5.1.41/src/lib/
mysql-connector-java-5.1.41/src/org/
mysql-connector-java-5.1.41/src/org/gjt/
mysql-connector-java-5.1.41/src/org/gjt/mm/
mysql-connector-java-5.1.41/src/org/gjt/mm/mysql/
mysql-connector-java-5.1.41/src/testsuite/
mysql-connector-java-5.1.41/src/testsuite/fabric/
mysql-connector-java-5.1.41/src/testsuite/fabric/jdbc/
mysql-connector-java-5.1.41/src/testsuite/perf/
mysql-connector-java-5.1.41/src/testsuite/regression/
mysql-connector-java-5.1.41/src/testsuite/regression/jdbc4/
mysql-connector-java-5.1.41/src/testsuite/regression/jdbc42/
mysql-connector-java-5.1.41/src/testsuite/simple/
mysql-connector-java-5.1.41/src/testsuite/simple/jdbc4/
mysql-connector-java-5.1.41/src/testsuite/simple/jdbc42/
mysql-connector-java-5.1.41/src/testsuite/ssl-test-certs/
mysql-connector-java-5.1.41/CHANGES
mysql-connector-java-5.1.41/COPYING
mysql-connector-java-5.1.41/README
mysql-connector-java-5.1.41/README.txt
mysql-connector-java-5.1.41/build.xml
mysql-connector-java-5.1.41/docs/README.txt
mysql-connector-java-5.1.41/docs/connector-j.html
mysql-connector-java-5.1.41/docs/connector-j.pdf
mysql-connector-java-5.1.41/mysql-connector-java-5.1.41-bin.jar
mysql-connector-java-5.1.41/src/com/mysql/fabric/FabricCommunicationException.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/FabricConnection.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/FabricStateResponse.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/HashShardMapping.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/RangeShardMapping.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/Response.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/Server.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/ServerGroup.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/ServerMode.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/ServerRole.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/ShardIndex.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/ShardMapping.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/ShardMappingFactory.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/ShardTable.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/ShardingType.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/hibernate/FabricMultiTenantConnectionProvider.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/jdbc/ErrorReportingExceptionInterceptor.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/jdbc/FabricMySQLConnection.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/jdbc/FabricMySQLConnectionProperties.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/jdbc/FabricMySQLConnectionProxy.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/jdbc/FabricMySQLDataSource.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/jdbc/FabricMySQLDriver.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/jdbc/JDBC4FabricMySQLConnection.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/jdbc/JDBC4FabricMySQLConnectionProxy.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/proto/xmlrpc/AuthenticatedXmlRpcMethodCaller.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/proto/xmlrpc/DigestAuthentication.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/proto/xmlrpc/InternalXmlRpcMethodCaller.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/proto/xmlrpc/ResultSetParser.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/proto/xmlrpc/XmlRpcClient.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/proto/xmlrpc/XmlRpcMethodCaller.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/xmlrpc/Client.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/xmlrpc/base/Array.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/xmlrpc/base/Data.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/xmlrpc/base/Fault.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/xmlrpc/base/Member.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/xmlrpc/base/MethodCall.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/xmlrpc/base/MethodResponse.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/xmlrpc/base/Param.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/xmlrpc/base/Params.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/xmlrpc/base/ResponseParser.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/xmlrpc/base/Struct.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/xmlrpc/base/Value.java
mysql-connector-java-5.1.41/src/com/mysql/fabric/xmlrpc/exceptions/MySQLFabricException.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/AbandonedConnectionCleanupThread.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/AssertionFailedException.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/AuthenticationPlugin.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/BalanceStrategy.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/BestResponseTimeBalanceStrategy.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/Blob.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/BlobFromLocator.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/Buffer.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/BufferRow.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/ByteArrayRow.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/CacheAdapter.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/CacheAdapterFactory.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/CachedResultSetMetaData.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/CallableStatement.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/CharsetMapping.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/Charsets.properties
mysql-connector-java-5.1.41/src/com/mysql/jdbc/Clob.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/CommunicationsException.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/CompressedInputStream.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/Connection.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/ConnectionFeatureNotAvailableException.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/ConnectionGroup.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/ConnectionGroupManager.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/ConnectionImpl.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/ConnectionLifecycleInterceptor.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/ConnectionProperties.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/ConnectionPropertiesImpl.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/ConnectionPropertiesTransform.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/Constants.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/DatabaseMetaData.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/DatabaseMetaDataUsingInfoSchema.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/DocsConnectionPropsHelper.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/Driver.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/EscapeProcessor.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/EscapeProcessorResult.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/EscapeTokenizer.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/ExceptionInterceptor.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/ExportControlled.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/Extension.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/FailoverConnectionProxy.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/Field.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/IterateBlock.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/JDBC42CallableStatement.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/JDBC42Helper.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/JDBC42PreparedStatement.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/JDBC42ResultSet.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/JDBC42ServerPreparedStatement.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/JDBC42UpdatableResultSet.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/JDBC4CallableStatement.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/JDBC4ClientInfoProvider.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/JDBC4ClientInfoProviderSP.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/JDBC4CommentClientInfoProvider.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/JDBC4Connection.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/JDBC4DatabaseMetaData.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/JDBC4DatabaseMetaDataUsingInfoSchema.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/JDBC4LoadBalancedMySQLConnection.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/JDBC4MultiHostMySQLConnection.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/JDBC4MySQLConnection.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/JDBC4MysqlSQLXML.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/JDBC4NClob.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/JDBC4PreparedStatement.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/JDBC4PreparedStatementHelper.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/JDBC4ReplicationMySQLConnection.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/JDBC4ResultSet.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/JDBC4ServerPreparedStatement.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/JDBC4UpdatableResultSet.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/LicenseConfiguration.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/LoadBalanceExceptionChecker.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/LoadBalancedAutoCommitInterceptor.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/LoadBalancedConnection.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/LoadBalancedConnectionProxy.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/LoadBalancedMySQLConnection.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/LocalizedErrorMessages.properties
mysql-connector-java-5.1.41/src/com/mysql/jdbc/Messages.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/MiniAdmin.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/MultiHostConnectionProxy.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/MultiHostMySQLConnection.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/MySQLConnection.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/MysqlDataTruncation.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/MysqlDefs.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/MysqlErrorNumbers.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/MysqlIO.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/MysqlParameterMetadata.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/MysqlSavepoint.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/NamedPipeSocketFactory.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/NdbLoadBalanceExceptionChecker.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/NetworkResources.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/NoSubInterceptorWrapper.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/NonRegisteringDriver.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/NonRegisteringReplicationDriver.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/NotImplemented.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/NotUpdatable.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/OperationNotSupportedException.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/OutputStreamWatcher.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/PacketTooBigException.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/ParameterBindings.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/PerConnectionLRUFactory.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/PerVmServerConfigCacheFactory.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/PingTarget.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/PreparedStatement.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/ProfilerEventHandlerFactory.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/RandomBalanceStrategy.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/ReflectiveStatementInterceptorAdapter.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/ReplicationConnection.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/ReplicationConnectionGroup.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/ReplicationConnectionGroupManager.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/ReplicationConnectionProxy.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/ReplicationDriver.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/ReplicationMySQLConnection.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/ResultSetImpl.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/ResultSetInternalMethods.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/ResultSetMetaData.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/ResultSetRow.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/RowData.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/RowDataCursor.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/RowDataDynamic.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/RowDataStatic.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/SQLError.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/Security.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/SequentialBalanceStrategy.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/ServerPreparedStatement.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/SingleByteCharsetConverter.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/SocketFactory.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/SocketMetadata.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/SocksProxySocketFactory.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/StandardLoadBalanceExceptionChecker.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/StandardSocketFactory.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/Statement.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/StatementImpl.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/StatementInterceptor.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/StatementInterceptorV2.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/StreamingNotifiable.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/StringUtils.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/TimeUtil.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/TimeZoneMapping.properties
mysql-connector-java-5.1.41/src/com/mysql/jdbc/UpdatableResultSet.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/Util.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/V1toV2StatementInterceptorAdapter.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/WatchableOutputStream.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/WatchableWriter.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/Wrapper.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/WriterWatcher.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/authentication/MysqlClearPasswordPlugin.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/authentication/MysqlNativePasswordPlugin.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/authentication/MysqlOldPasswordPlugin.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/authentication/Sha256PasswordPlugin.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/configs/3-0-Compat.properties
mysql-connector-java-5.1.41/src/com/mysql/jdbc/configs/5-0-Compat.properties
mysql-connector-java-5.1.41/src/com/mysql/jdbc/configs/clusterBase.properties
mysql-connector-java-5.1.41/src/com/mysql/jdbc/configs/coldFusion.properties
mysql-connector-java-5.1.41/src/com/mysql/jdbc/configs/fullDebug.properties
mysql-connector-java-5.1.41/src/com/mysql/jdbc/configs/maxPerformance.properties
mysql-connector-java-5.1.41/src/com/mysql/jdbc/configs/solarisMaxPerformance.properties
mysql-connector-java-5.1.41/src/com/mysql/jdbc/exceptions/DeadlockTimeoutRollbackMarker.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/exceptions/MySQLDataException.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/exceptions/MySQLIntegrityConstraintViolationException.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/exceptions/MySQLInvalidAuthorizationSpecException.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/exceptions/MySQLNonTransientConnectionException.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/exceptions/MySQLNonTransientException.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/exceptions/MySQLQueryInterruptedException.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/exceptions/MySQLStatementCancelledException.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/exceptions/MySQLSyntaxErrorException.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/exceptions/MySQLTimeoutException.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/exceptions/MySQLTransactionRollbackException.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/exceptions/MySQLTransientConnectionException.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/exceptions/MySQLTransientException.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/exceptions/jdbc4/CommunicationsException.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/exceptions/jdbc4/MySQLDataException.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/exceptions/jdbc4/MySQLIntegrityConstraintViolationException.ja                                                                                                                  va
mysql-connector-java-5.1.41/src/com/mysql/jdbc/exceptions/jdbc4/MySQLInvalidAuthorizationSpecException.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/exceptions/jdbc4/MySQLNonTransientConnectionException.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/exceptions/jdbc4/MySQLNonTransientException.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/exceptions/jdbc4/MySQLQueryInterruptedException.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/exceptions/jdbc4/MySQLSyntaxErrorException.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/exceptions/jdbc4/MySQLTimeoutException.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/exceptions/jdbc4/MySQLTransactionRollbackException.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/exceptions/jdbc4/MySQLTransientConnectionException.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/exceptions/jdbc4/MySQLTransientException.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/integration/c3p0/MysqlConnectionTester.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/integration/jboss/ExtendedMysqlExceptionSorter.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/integration/jboss/MysqlValidConnectionChecker.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/interceptors/ResultSetScannerInterceptor.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/interceptors/ServerStatusDiffInterceptor.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/interceptors/SessionAssociationInterceptor.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/jdbc2/optional/CallableStatementWrapper.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/jdbc2/optional/ConnectionWrapper.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/jdbc2/optional/JDBC42CallableStatementWrapper.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/jdbc2/optional/JDBC42PreparedStatementWrapper.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/jdbc2/optional/JDBC4CallableStatementWrapper.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/jdbc2/optional/JDBC4ConnectionWrapper.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/jdbc2/optional/JDBC4MysqlPooledConnection.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/jdbc2/optional/JDBC4MysqlXAConnection.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/jdbc2/optional/JDBC4PreparedStatementWrapper.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/jdbc2/optional/JDBC4StatementWrapper.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/jdbc2/optional/JDBC4SuspendableXAConnection.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/jdbc2/optional/MysqlConnectionPoolDataSource.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/jdbc2/optional/MysqlDataSource.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/jdbc2/optional/MysqlDataSourceFactory.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/jdbc2/optional/MysqlPooledConnection.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/jdbc2/optional/MysqlXAConnection.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/jdbc2/optional/MysqlXADataSource.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/jdbc2/optional/MysqlXAException.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/jdbc2/optional/MysqlXid.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/jdbc2/optional/PreparedStatementWrapper.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/jdbc2/optional/StatementWrapper.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/jdbc2/optional/SuspendableXAConnection.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/jdbc2/optional/WrapperBase.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/jmx/LoadBalanceConnectionGroupManager.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/jmx/LoadBalanceConnectionGroupManagerMBean.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/jmx/ReplicationGroupManager.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/jmx/ReplicationGroupManagerMBean.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/log/Jdk14Logger.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/log/Log.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/log/LogFactory.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/log/LogUtils.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/log/NullLogger.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/log/Slf4JLogger.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/log/StandardLogger.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/profiler/LoggingProfilerEventHandler.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/profiler/ProfilerEvent.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/profiler/ProfilerEventHandler.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/util/Base64Decoder.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/util/BaseBugReport.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/util/ErrorMappingsDocGenerator.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/util/LRUCache.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/util/PropertiesDocGenerator.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/util/ReadAheadInputStream.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/util/ResultSetUtil.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/util/ServerController.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/util/TimezoneDump.java
mysql-connector-java-5.1.41/src/com/mysql/jdbc/util/VersionFSHierarchyMaker.java
mysql-connector-java-5.1.41/src/demo/fabric/Client1_Fabric.java
mysql-connector-java-5.1.41/src/demo/fabric/Employee.java
mysql-connector-java-5.1.41/src/demo/fabric/EmployeesDataSource.java
mysql-connector-java-5.1.41/src/demo/fabric/EmployeesJdbc.java
mysql-connector-java-5.1.41/src/demo/fabric/HibernateFabric.java
mysql-connector-java-5.1.41/src/demo/fabric/resources/com/mysql/fabric/demo/employee.hbm.xml
mysql-connector-java-5.1.41/src/doc/sources/pom.xml
mysql-connector-java-5.1.41/src/lib/c3p0-0.9.1-pre6.jar
mysql-connector-java-5.1.41/src/lib/c3p0-0.9.1-pre6.src.zip
mysql-connector-java-5.1.41/src/lib/jboss-common-jdbc-wrapper-src.jar
mysql-connector-java-5.1.41/src/lib/jboss-common-jdbc-wrapper.jar
mysql-connector-java-5.1.41/src/lib/slf4j-api-1.6.1.jar
mysql-connector-java-5.1.41/src/org/gjt/mm/mysql/Driver.java
mysql-connector-java-5.1.41/src/testsuite/BaseStatementInterceptor.java
mysql-connector-java-5.1.41/src/testsuite/BaseTestCase.java
mysql-connector-java-5.1.41/src/testsuite/UnreliableSocketFactory.java
mysql-connector-java-5.1.41/src/testsuite/fabric/BaseFabricTestCase.java
mysql-connector-java-5.1.41/src/testsuite/fabric/SetupFabricTestsuite.java
mysql-connector-java-5.1.41/src/testsuite/fabric/TestAdminCommands.java
mysql-connector-java-5.1.41/src/testsuite/fabric/TestDumpCommands.java
mysql-connector-java-5.1.41/src/testsuite/fabric/TestResultSetParser.java
mysql-connector-java-5.1.41/src/testsuite/fabric/TestShardMapping.java
mysql-connector-java-5.1.41/src/testsuite/fabric/TestXmlRpcCore.java
mysql-connector-java-5.1.41/src/testsuite/fabric/jdbc/TestBasicConnection.java
mysql-connector-java-5.1.41/src/testsuite/fabric/jdbc/TestFabricMySQLConnectionSharding.java
mysql-connector-java-5.1.41/src/testsuite/fabric/jdbc/TestHABasics.java
mysql-connector-java-5.1.41/src/testsuite/fabric/jdbc/TestHashSharding.java
mysql-connector-java-5.1.41/src/testsuite/fabric/jdbc/TestRegressions.java
mysql-connector-java-5.1.41/src/testsuite/perf/BasePerfTest.java
mysql-connector-java-5.1.41/src/testsuite/perf/LoadStorePerfTest.java
mysql-connector-java-5.1.41/src/testsuite/perf/RetrievalPerfTest.java
mysql-connector-java-5.1.41/src/testsuite/regression/BlobRegressionTest.java
mysql-connector-java-5.1.41/src/testsuite/regression/CachedRowsetTest.java
mysql-connector-java-5.1.41/src/testsuite/regression/CallableStatementRegressionTest.java
mysql-connector-java-5.1.41/src/testsuite/regression/CharsetRegressionTest.java
mysql-connector-java-5.1.41/src/testsuite/regression/ConnectionRegressionTest.java
mysql-connector-java-5.1.41/src/testsuite/regression/DataSourceRegressionTest.java
mysql-connector-java-5.1.41/src/testsuite/regression/EscapeProcessorRegressionTest.java
mysql-connector-java-5.1.41/src/testsuite/regression/MetaDataRegressionTest.java
mysql-connector-java-5.1.41/src/testsuite/regression/MicroPerformanceRegressionTest.java
mysql-connector-java-5.1.41/src/testsuite/regression/NumbersRegressionTest.java
mysql-connector-java-5.1.41/src/testsuite/regression/PooledConnectionRegressionTest.java
mysql-connector-java-5.1.41/src/testsuite/regression/ResultSetRegressionTest.java
mysql-connector-java-5.1.41/src/testsuite/regression/StatementRegressionTest.java
mysql-connector-java-5.1.41/src/testsuite/regression/StressRegressionTest.java
mysql-connector-java-5.1.41/src/testsuite/regression/StringRegressionTest.java
mysql-connector-java-5.1.41/src/testsuite/regression/SubqueriesRegressionTest.java
mysql-connector-java-5.1.41/src/testsuite/regression/SyntaxRegressionTest.java
mysql-connector-java-5.1.41/src/testsuite/regression/UtilsRegressionTest.java
mysql-connector-java-5.1.41/src/testsuite/regression/jdbc4/ConnectionRegressionTest.java
mysql-connector-java-5.1.41/src/testsuite/regression/jdbc4/ExceptionSubclassesTest.java
mysql-connector-java-5.1.41/src/testsuite/regression/jdbc4/MetaDataRegressionTest.java
mysql-connector-java-5.1.41/src/testsuite/regression/jdbc4/StatementRegressionTest.java
mysql-connector-java-5.1.41/src/testsuite/regression/jdbc42/ConnectionRegressionTest.java
mysql-connector-java-5.1.41/src/testsuite/regression/jdbc42/StatementRegressionTest.java
mysql-connector-java-5.1.41/src/testsuite/simple/BlobTest.java
mysql-connector-java-5.1.41/src/testsuite/simple/CallableStatementTest.java
mysql-connector-java-5.1.41/src/testsuite/simple/CharsetTest.java
mysql-connector-java-5.1.41/src/testsuite/simple/ConnectionTest.java
mysql-connector-java-5.1.41/src/testsuite/simple/DataSourceTest.java
mysql-connector-java-5.1.41/src/testsuite/simple/DateTest.java
mysql-connector-java-5.1.41/src/testsuite/simple/EscapeProcessingTest.java
mysql-connector-java-5.1.41/src/testsuite/simple/MetadataTest.java
mysql-connector-java-5.1.41/src/testsuite/simple/MiniAdminTest.java
mysql-connector-java-5.1.41/src/testsuite/simple/MultiHostConnectionTest.java
mysql-connector-java-5.1.41/src/testsuite/simple/NumbersTest.java
mysql-connector-java-5.1.41/src/testsuite/simple/ReadOnlyCallableStatementTest.java
mysql-connector-java-5.1.41/src/testsuite/simple/ResultSetTest.java
mysql-connector-java-5.1.41/src/testsuite/simple/SSLTest.java
mysql-connector-java-5.1.41/src/testsuite/simple/ServerControllerTest.java
mysql-connector-java-5.1.41/src/testsuite/simple/SimpleTransformer.java
mysql-connector-java-5.1.41/src/testsuite/simple/SplitDBdotNameTest.java
mysql-connector-java-5.1.41/src/testsuite/simple/StatementsTest.java
mysql-connector-java-5.1.41/src/testsuite/simple/StringUtilsTest.java
mysql-connector-java-5.1.41/src/testsuite/simple/TestBug57662Logger.java
mysql-connector-java-5.1.41/src/testsuite/simple/TestLifecycleInterceptor.java
mysql-connector-java-5.1.41/src/testsuite/simple/TransactionTest.java
mysql-connector-java-5.1.41/src/testsuite/simple/TraversalTest.java
mysql-connector-java-5.1.41/src/testsuite/simple/UpdatabilityTest.java
mysql-connector-java-5.1.41/src/testsuite/simple/UtilsTest.java
mysql-connector-java-5.1.41/src/testsuite/simple/XATest.java
mysql-connector-java-5.1.41/src/testsuite/simple/jdbc4/StatementsTest.java
mysql-connector-java-5.1.41/src/testsuite/simple/jdbc42/ConnectionTest.java
mysql-connector-java-5.1.41/src/testsuite/simple/jdbc42/ResultSetTest.java
mysql-connector-java-5.1.41/src/testsuite/simple/jdbc42/StatementsTest.java
mysql-connector-java-5.1.41/src/testsuite/simple/tb2-data.txt.gz
mysql-connector-java-5.1.41/src/testsuite/ssl-test-certs/ca-cert.pem
mysql-connector-java-5.1.41/src/testsuite/ssl-test-certs/ca-key.pem
mysql-connector-java-5.1.41/src/testsuite/ssl-test-certs/certs_howto.txt
mysql-connector-java-5.1.41/src/testsuite/ssl-test-certs/mykey.pem
mysql-connector-java-5.1.41/src/testsuite/ssl-test-certs/mykey.pub
mysql-connector-java-5.1.41/src/testsuite/ssl-test-certs/server-cert.pem
mysql-connector-java-5.1.41/src/testsuite/ssl-test-certs/server-key.pem
mysql-connector-java-5.1.41/src/testsuite/ssl-test-certs/server-req.pem
mysql-connector-java-5.1.41/src/testsuite/ssl-test-certs/test-cert-store
[root@ip-172-31-7-179 ec2-user]# yum install oracle-j2sdk1.7
Loaded plugins: amazon-id, rhui-lb, search-disabled-repos
No package oracle-j2sdk1.7 available.
Error: Nothing to do
[root@ip-172-31-7-179 ec2-user]# vi /etc/yum.
yum.conf     yum.repos.d/
[root@ip-172-31-7-179 ec2-user]# vi /etc/yum.repos.d/cloudera-manager.repo
[root@ip-172-31-7-179 ec2-user]# vi /etc/yum.repos.d/cloudera-manager.repo
[root@ip-172-31-7-179 ec2-user]# yum clean all
Loaded plugins: amazon-id, rhui-lb, search-disabled-repos
Config error: File contains no section headers.
file: file:///etc/yum.repos.d/cloudera-manager.repo, line: 2
'udera-manager]\n'
[root@ip-172-31-7-179 ec2-user]# vi /etc/yum.repos.d/cloudera-manager.repo
[root@ip-172-31-7-179 ec2-user]# yum clean all
Loaded plugins: amazon-id, rhui-lb, search-disabled-repos
Cleaning repos: cloudera-manager epel mysql-connectors-community mysql-tools-community mysql56-community
              : rhui-REGION-client-config-server-7 rhui-REGION-rhel-server-releases
              : rhui-REGION-rhel-server-rh-common
Cleaning up everything
[root@ip-172-31-7-179 ec2-user]# yum install oracle-j2sdk1.7
Loaded plugins: amazon-id, rhui-lb, search-disabled-repos
cloudera-manager                                                                      |  951 B  00:00:00
epel/x86_64/metalink                                                                  |  22 kB  00:00:00
epel                                                                                  | 4.3 kB  00:00:00
mysql-connectors-community                                                            | 2.5 kB  00:00:00
mysql-tools-community                                                                 | 2.5 kB  00:00:00
mysql56-community                                                                     | 2.5 kB  00:00:00
rhui-REGION-client-config-server-7                                                    | 2.9 kB  00:00:00
rhui-REGION-rhel-server-releases                                                      | 3.5 kB  00:00:00
rhui-REGION-rhel-server-rh-common                                                     | 3.8 kB  00:00:00
(1/13): epel/x86_64/group_gz                                                          | 170 kB  00:00:00
(2/13): epel/x86_64/updateinfo                                                        | 753 kB  00:00:00
(3/13): epel/x86_64/primary_db                                                        | 4.6 MB  00:00:00
(4/13): mysql56-community/x86_64/primary_db                                           | 159 kB  00:00:00
(5/13): mysql-tools-community/x86_64/primary_db                                       |  32 kB  00:00:00
(6/13): mysql-connectors-community/x86_64/primary_db                                  |  13 kB  00:00:00
(7/13): rhui-REGION-client-config-server-7/x86_64/primary_db                          | 4.3 kB  00:00:00
(8/13): rhui-REGION-rhel-server-rh-common/7Server/x86_64/updateinfo                   |  29 kB  00:00:00
(9/13): rhui-REGION-rhel-server-releases/7Server/x86_64/updateinfo                    | 1.8 MB  00:00:00
(10/13): rhui-REGION-rhel-server-releases/7Server/x86_64/group                        | 701 kB  00:00:00
(11/13): rhui-REGION-rhel-server-rh-common/7Server/x86_64/group                       |  104 B  00:00:00
(12/13): rhui-REGION-rhel-server-rh-common/7Server/x86_64/primary_db                  | 110 kB  00:00:00
(13/13): rhui-REGION-rhel-server-releases/7Server/x86_64/primary_db                   |  34 MB  00:00:00
cloudera-manager/primary                                                              | 4.3 kB  00:00:00
cloudera-manager                                                                                         8/8
Resolving Dependencies
--> Running transaction check
---> Package oracle-j2sdk1.7.x86_64 0:1.7.0+update67-1 will be installed
--> Finished Dependency Resolution

Dependencies Resolved

=============================================================================================================
 Package                    Arch              Version                      Repository                   Size
=============================================================================================================
Installing:
 oracle-j2sdk1.7            x86_64            1.7.0+update67-1             cloudera-manager            135 M

Transaction Summary
=============================================================================================================
Install  1 Package

Total download size: 135 M
Installed size: 279 M
Is this ok [y/d/N]: y
Downloading packages:
warning: /var/cache/yum/x86_64/7Server/cloudera-manager/packages/oracle-j2sdk1.7-1.7.0+update67-1.x86_64.rpm:                                                                                                                   Header V4 DSA/SHA1 Signature, key ID e8f86acd: NOKEY
Public key for oracle-j2sdk1.7-1.7.0+update67-1.x86_64.rpm is not installed
oracle-j2sdk1.7-1.7.0+update67-1.x86_64.rpm                                           | 135 MB  00:00:03
Retrieving key from https://archive.cloudera.com/cm5/redhat/5/x86_64/cm/RPM-GPG-KEY-cloudera
Importing GPG key 0xE8F86ACD:
 Userid     : "Yum Maintainer <webmaster@cloudera.com>"
 Fingerprint: 5f14 d39e f068 1aca 6f04 4a43 f90c 0d8f e8f8 6acd
 From       : https://archive.cloudera.com/cm5/redhat/5/x86_64/cm/RPM-GPG-KEY-cloudera
Is this ok [y/N]: y
Running transaction check
Running transaction test
Transaction test succeeded
Running transaction
  Installing : oracle-j2sdk1.7-1.7.0+update67-1.x86_64                                                   1/1
  Verifying  : oracle-j2sdk1.7-1.7.0+update67-1.x86_64                                                   1/1

Installed:
  oracle-j2sdk1.7.x86_64 0:1.7.0+update67-1

Complete!
[root@ip-172-31-7-179 ec2-user]# cp mysql-connector-java-5.1.41/mysql-connector-java-5.1.41                                                                                                                                    -bin.jar /usr/share/
aclocal/                     gnupg/                       polkit-1/
anaconda/                    groff/                       pygobject/
applications/                grub/                        python-dmidecode/
augeas/                      hwdata/                      redhat-logos/
authconfig/                  i18n/                        redhat-release/
awk/                         icons/                       rhn/
backgrounds/                 idl/                         rhsm/
bash-completion/             info/                        rhsm-plugins/
cracklib/                    kde4/                        selinux/
dbus-1/                      kdump/                       setools-3.3/
desktop-directories/         licenses/                    setuptool/
dict/                        locale/                      sounds/
doc/                         lua/                         systemd/
emacs/                       magic                        systemtap/
empty/                       man/                         tabset/
file/                        mime/                        terminfo/
firstboot/                   mime-info/                   themes/
games/                       misc/                        tuned/
gcc-4.8.2/                   mysql/                       wallpapers/
gcc-4.8.5/                   omf/                         X11/
GConf/                       os-prober/                   xsessions/
gdb/                         p11-kit/                     yum-cli/
gettext/                     perl5/                       yum-plugins/
ghostscript/                 pixmaps/                     zoneinfo/
glib-2.0/                    pkgconfig/                   zsh/
gnome/                       pki/
gnome-background-properties/ plymouth/
[root@ip-172-31-7-179 ec2-user]# mkdir -p /usr/share/java
[root@ip-172-31-7-179 ec2-user]# cp mysql-connector-java-5.1.41
mysql-connector-java-5.1.41/        mysql-connector-java-5.1.41.tar.gz
[root@ip-172-31-7-179 ec2-user]# cp mysql-connector-java-5.1.41/mysql-connector-java-5.1.41                                                                                                                                    -bin.jar /usr/share/java/mysql-connector-java.jar
[root@ip-172-31-7-179 ec2-user]# /usr/bin/my
myisamchk                   mysqlaccess                 mysql_convert_table_format  mysql_fix_extensions        mysqlshow                   mysql_waitpid
myisam_ftdump               mysqladmin                  mysqld_multi                mysqlhotcopy                mysqlslap                   mysql_zap
myisamlog                   mysqlbinlog                 mysqld_safe                 mysqlimport                 mysql-systemd-start
myisampack                  mysqlbug                    mysqldump                   mysql_install_db            mysqltest
my_print_defaults           mysqlcheck                  mysqldumpslow               mysql_plugin                mysql_tzinfo_to_sql
mysql                       mysql_config_editor         mysql_find_rows             mysql_secure_installation   mysql_upgrade
[root@ip-172-31-7-179 ec2-user]# /usr/bin/my
myisamchk                   mysqlaccess                 mysql_convert_table_format  mysql_fix_extensions        mysqlshow                   mysql_waitpid
myisam_ftdump               mysqladmin                  mysqld_multi                mysqlhotcopy                mysqlslap                   mysql_zap
myisamlog                   mysqlbinlog                 mysqld_safe                 mysqlimport                 mysql-systemd-start
myisampack                  mysqlbug                    mysqldump                   mysql_install_db            mysqltest
my_print_defaults           mysqlcheck                  mysqldumpslow               mysql_plugin                mysql_tzinfo_to_sql
mysql                       mysql_config_editor         mysql_find_rows             mysql_secure_installation   mysql_upgrade
[root@ip-172-31-7-179 ec2-user]# /usr/bin/mysql_secure_installation



NOTE: RUNNING ALL PARTS OF THIS SCRIPT IS RECOMMENDED FOR ALL MySQL
      SERVERS IN PRODUCTION USE!  PLEASE READ EACH STEP CAREFULLY!

In order to log into MySQL to secure it, we'll need the current
password for the root user.  If you've just installed MySQL, and
you haven't set the root password yet, the password will be blank,
so you should just press enter here.

Enter current password for root (enter for none):
ERROR 2002 (HY000): Can't connect to local MySQL server through socket '/var/lib/mysql/mysql.sock' (2)
Enter current password for root (enter for none):
ERROR 2002 (HY000): Can't connect to local MySQL server through socket '/var/lib/mysql/mysql.sock' (2)
Enter current password for root (enter for none):
ERROR 2002 (HY000): Can't connect to local MySQL server through socket '/var/lib/mysql/mysql.sock' (2)
Unable to connect to the server as root user, giving up.
Cleaning up...
[root@ip-172-31-7-179 ec2-user]# mysql -u root -p
Enter password:
ERROR 2002 (HY000): Can't connect to local MySQL server through socket '/var/lib/mysql/mysql.sock' (2)
[root@ip-172-31-7-179 ec2-user]# mysql -u root -p
Enter password:
ERROR 2002 (HY000): Can't connect to local MySQL server through socket '/var/lib/mysql/mysql.sock' (2)
[root@ip-172-31-7-179 ec2-user]#
[root@ip-172-31-7-179 ec2-user]# mysql -u root -p
Enter password:
ERROR 2002 (HY000): Can't connect to local MySQL server through socket '/var/lib/mysql/mysql.sock' (2)
[root@ip-172-31-7-179 ec2-user]# mysql
ERROR 2002 (HY000): Can't connect to local MySQL server through socket '/var/lib/mysql/mysql.sock' (2)
[root@ip-172-31-7-179 ec2-user]# service mysqld start
Redirecting to /bin/systemctl start  mysqld.service
[root@ip-172-31-7-179 ec2-user]# /usr/bin/mysql_secure_installation



NOTE: RUNNING ALL PARTS OF THIS SCRIPT IS RECOMMENDED FOR ALL MySQL
      SERVERS IN PRODUCTION USE!  PLEASE READ EACH STEP CAREFULLY!

In order to log into MySQL to secure it, we'll need the current
password for the root user.  If you've just installed MySQL, and
you haven't set the root password yet, the password will be blank,
so you should just press enter here.

Enter current password for root (enter for none):
OK, successfully used password, moving on...

Setting the root password ensures that nobody can log into the MySQL
root user without the proper authorisation.

Set root password? [Y/n] Y
New password:
Re-enter new password:
Password updated successfully!
Reloading privilege tables..
 ... Success!


By default, a MySQL installation has an anonymous user, allowing anyone
to log into MySQL without having to have a user account created for
them.  This is intended only for testing, and to make the installation
go a bit smoother.  You should remove them before moving into a
production environment.

Remove anonymous users? [Y/n] Y
 ... Success!

Normally, root should only be allowed to connect from 'localhost'.  This
ensures that someone cannot guess at the root password from the network.

Disallow root login remotely? [Y/n] n
 ... skipping.

By default, MySQL comes with a database named 'test' that anyone can
access.  This is also intended only for testing, and should be removed
before moving into a production environment.

Remove test database and access to it? [Y/n] Y
 - Dropping test database...
ERROR 1008 (HY000) at line 1: Can't drop database 'test'; database doesn't exist
 ... Failed!  Not critical, keep moving...
 - Removing privileges on test database...
 ... Success!

Reloading the privilege tables will ensure that all changes made so far
will take effect immediately.

Reload privilege tables now? [Y/n] Y
 ... Success!




All done!  If you've completed all of the above steps, your MySQL
installation should now be secure.

Thanks for using MySQL!


Cleaning up...
