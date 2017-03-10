##listing
```
[hdfs@sk-node2 cloudera-scm-server]$ hadoop fs -ls /
Found 2 items
drwxrwxrwt   - hdfs supergroup          0 2017-03-10 05:13 /tmp
drwxr-xr-x   - hdfs supergroup          0 2017-03-10 05:13 /user
[hdfs@sk-node2 cloudera-scm-server]$ hadoop fs -mkdir /user/neymar
[hdfs@sk-node2 cloudera-scm-server]$ hadoop fs -mkdir /user/ronaldo
````
##api
```

[hdfs@sk-node2 cloudera-scm-server]$ curl sebastiankramp:cloudera@localhost:7180/api/v14/hosts/
{
  "items" : [ {
    "hostId" : "i-0ae6bdbfce2fa212b",
    "ipAddress" : "172.31.7.179",
    "hostname" : "SK-Node1",
    "rackId" : "/default",
    "hostUrl" : "http://SK-Node2:7180/cmf/hostRedirect/i-0ae6bdbfce2fa212b",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332438016
  }, {
    "hostId" : "i-0c0e14303dac48e5f",
    "ipAddress" : "172.31.6.8",
    "hostname" : "SK-Node2",
    "rackId" : "/default",
    "hostUrl" : "http://SK-Node2:7180/cmf/hostRedirect/i-0c0e14303dac48e5f",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332438016
  }, {
    "hostId" : "i-0cb74c69727a870f1",
    "ipAddress" : "172.31.0.171",
    "hostname" : "SK-Node3",
    "rackId" : "/default",
    "hostUrl" : "http://SK-Node2:7180/cmf/hostRedirect/i-0cb74c69727a870f1",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332438016
  }, {
    "hostId" : "i-0d415597b1cd08553",
    "ipAddress" : "172.31.9.231",
    "hostname" : "SK-Node4",
    "rackId" : "/default",
    "hostUrl" : "http://SK-Node2:7180/cmf/hostRedirect/i-0d415597b1cd08553",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332438016
  }, {
    "hostId" : "i-0e69a4ca1a6909cdc",
    "ipAddress" : "172.31.4.146",
    "hostname" : "SK-Node5",
    "rackId" : "/default",
    "hostUrl" : "http://SK-Node2:7180/cmf/hostRedirect/i-0e69a4ca1a6909cdc",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332438016
  } ]
}[hdfs@sk-node2 cloudera-scm-server]$

```