#HIVE API

##Status
curl sebastiankramp:cloudera@localhost:7180/api/v11/clusterssebastiankramp/services/hive/  
```json{
  "name" : "hive",
  "type" : "HIVE",
  "clusterRef" : {
    "clusterName" : "cluster"
  },
  "serviceUrl" : "http://ec2-54-191-166-77.us-west-2.compute.amazonaws.com:7180/cmf/serviceRedirect/hive",
  "roleInstancesUrl" : "http://ec2-54-191-166-77.us-west-2.compute.amazonaws.com:7180/cmf/serviceRedirect/hive/instances",
  "serviceState" : "STARTED",
  "healthSummary" : "GOOD",
  "healthChecks" : [ {
    "name" : "HIVE_HIVEMETASTORES_HEALTHY",
    "summary" : "GOOD",
    "suppressed" : false
  }, {
    "name" : "HIVE_HIVESERVER2S_HEALTHY",
    "summary" : "GOOD",
    "suppressed" : false
  } ],
  "configStalenessStatus" : "FRESH",
  "clientConfigStalenessStatus" : "FRESH",
  "maintenanceMode" : false,
  "maintenanceOwners" : [ ],
  "displayName" : "Hive",
  "entityStatus" : "GOOD_HEALTH"```

##start
curl -X POST sebastiankramp:cloudera@localhost:7180/api/v11/clusters/sebastiankramp/services/hive/commands/start
```json{
  "id" : 1364,
  "name" : "Start",
  "startTime" : "2017-03-08T10:18:46.553Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }```


##stop
curl -X POST sebastiankramp:cloudera@localhost:7180/api/v11/clusters/sebastiankramp/services/hive/commands/stop
```json{
  "id" : 1361,
  "name" : "Stop",
  "startTime" : "2017-03-08T10:18:14.510Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }```


