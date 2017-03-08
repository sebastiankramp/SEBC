#Treasure Hunt

#What is ubertask optimization?
Whether to enable ubertask optimization, which runs "sufficiently small" jobs sequentially within a single JVM. "Small" is defined by the mapreduce.job.ubertask.maxmaps, mapreduce.job.ubertask.maxreduces, and mapreduce.job.ubertask.maxbytes settings.

#Where in CM is the Kerberos Security Realm value displayed?
Search: default_realm
Administration - Settings - Kerberos

#Which CDH service(s) host a property for enabling Kerberos authentication?
Zookeeper, Hive, Hue, Oozie, HDFS, CMS

#How do you upgrade the CM agents?
with the wizzard

#Give the tsquery statement used to chart Hue's CPU utilization?
select cpu_user_rate / getHostFact(numCores, 1) * 100, cpu_system_rate / getHostFact(numCores, 1) * 100, cpu_nice_rate / getHostFact(numCores, 1) * 100, cpu_iowait_rate / getHostFact(numCores, 1) * 100, cpu_irq_rate / getHostFact(numCores, 1) * 100, cpu_soft_irq_rate / getHostFact(numCores, 1) * 100, cpu_steal_rate / getHostFact(numCores, 1) * 100 where entityName=$HOSTID

#Name all the roles that make up the Hive service
Gateway
Hive Metastore Server
HiveServer2
WebHCat Server

#What steps must be completed before integrating Cloudera Manager with Kerberos?
- Set up a working KDC. Cloudera Manager supports MIT KDC and Active Directory.
- The KDC should be configured to have non-zero ticket lifetime and renewal lifetime. CDH will not work properly if tickets are not renewable.
- OpenLdap client libraries should be installed on the Cloudera Manager Server host if you want to use Active Directory. Also, Kerberos client libraries should be installed on ALL hosts.
- Cloudera Manager needs an account that has permissions to create other accounts in the KDC.
