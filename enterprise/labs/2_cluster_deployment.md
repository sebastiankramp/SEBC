


#CURL

##command
curl sebastiankramp:cloudera@localhost:7180/api/v2/cm/deployment > /home/hdfs/log.txt


##output
```json{
  "timestamp" : "2017-03-08T09:58:06.219Z",
  "clusters" : [ {
    "name" : "sebastiankramp",
    "version" : "CDH5",
    "services" : [ {
      "name" : "hive",
      "type" : "HIVE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "HIVEMETASTORE",
          "items" : [ {
            "name" : "hive_metastore_java_heapsize",
            "value" : "593494016"
          } ]
        }, {
          "roleType" : "HIVESERVER2",
          "items" : [ {
            "name" : "hiveserver2_java_heapsize",
            "value" : "593494016"
          }, {
            "name" : "hiveserver2_spark_driver_memory",
            "value" : "966367641"
          }, {
            "name" : "hiveserver2_spark_executor_cores",
            "value" : "4"
          }, {
            "name" : "hiveserver2_spark_executor_memory",
            "value" : "3433247539"
          }, {
            "name" : "hiveserver2_spark_yarn_driver_memory_overhead",
            "value" : "102"
          }, {
            "name" : "hiveserver2_spark_yarn_executor_memory_overhead",
            "value" : "577"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_metastore_database_host",
          "value" : "ip-172-31-0-164.eu-central-1.compute.internal"
        }, {
          "name" : "hive_metastore_database_name",
          "value" : "hive"
        }, {
          "name" : "hive_metastore_database_password",
          "value" : "cloudera"
        }, {
          "name" : "hive_metastore_database_user",
          "value" : "root"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hive-GATEWAY-0bef6295e924612353f8a8bd0c276f19",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-0a1da5f86407b0799"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-410863ccd3100e57b635ec541acb8d9d",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-048ee553725f66843"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-7cce873b6e102ea67626e37de8acb787",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-09b9b81d5c51f2ce7"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-bcae5707b2963b28316034c1fd2dabf4",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-0cf9327bd671c8b3b"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-c3b7a8e02b04a8dc19451f367409d9f6",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-07311d22df2d63466"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-HIVEMETASTORE-410863ccd3100e57b635ec541acb8d9d",
        "type" : "HIVEMETASTORE",
        "hostRef" : {
          "hostId" : "i-048ee553725f66843"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6kdxzb3bip85go9m5a9yb98bg"
          } ]
        }
      }, {
        "name" : "hive-HIVESERVER2-410863ccd3100e57b635ec541acb8d9d",
        "type" : "HIVESERVER2",
        "hostRef" : {
          "hostId" : "i-048ee553725f66843"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6bz7l0n6cusvk40kps9u2iiah"
          } ]
        }
      } ],
      "displayName" : "Hive"
    }, {
      "name" : "zookeeper",
      "type" : "ZOOKEEPER",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "SERVER",
          "items" : [ {
            "name" : "zookeeper_server_java_heapsize",
            "value" : "593494016"
          } ]
        } ],
        "items" : [ ]
      },
      "roles" : [ {
        "name" : "zookeeper-SERVER-0bef6295e924612353f8a8bd0c276f19",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "i-0a1da5f86407b0799"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "52z5q21gvrpw1d8qj7cgtbqei"
          }, {
            "name" : "serverId",
            "value" : "2"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-410863ccd3100e57b635ec541acb8d9d",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "i-048ee553725f66843"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "56irtkq1kjur8hnqn6xwcrcn1"
          }, {
            "name" : "serverId",
            "value" : "1"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-7cce873b6e102ea67626e37de8acb787",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "i-09b9b81d5c51f2ce7"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "et59lsrbnyzew9moywvjpwe6s"
          }, {
            "name" : "serverId",
            "value" : "3"
          } ]
        }
      } ],
      "displayName" : "ZooKeeper"
    }, {
      "name" : "hue",
      "type" : "HUE",
      "config" : {
        "roleTypeConfigs" : [ ],
        "items" : [ {
          "name" : "database_host",
          "value" : "ip-172-31-0-164.eu-central-1.compute.internal"
        }, {
          "name" : "database_password",
          "value" : "cloudera"
        }, {
          "name" : "database_type",
          "value" : "mysql"
        }, {
          "name" : "database_user",
          "value" : "root"
        }, {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "hue_webhdfs",
          "value" : "hdfs-HTTPFS-410863ccd3100e57b635ec541acb8d9d"
        }, {
          "name" : "oozie_service",
          "value" : "oozie"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hue-HUE_SERVER-410863ccd3100e57b635ec541acb8d9d",
        "type" : "HUE_SERVER",
        "hostRef" : {
          "hostId" : "i-048ee553725f66843"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "djo76538yhnuhwc6qhdi1ag"
          }, {
            "name" : "secret_key",
            "value" : "KLcsq03WHHkxnUDhhy0R4Mpx5NimWV"
          } ]
        }
      } ],
      "displayName" : "Hue"
    }, {
      "name" : "oozie",
      "type" : "OOZIE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "OOZIE_SERVER",
          "items" : [ {
            "name" : "oozie_database_host",
            "value" : "ip-172-31-0-164.eu-central-1.compute.internal"
          }, {
            "name" : "oozie_database_password",
            "value" : "cloudera"
          }, {
            "name" : "oozie_database_type",
            "value" : "mysql"
          }, {
            "name" : "oozie_database_user",
            "value" : "root"
          }, {
            "name" : "oozie_java_heapsize",
            "value" : "593494016"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "oozie_upload_sharelib_cmd_timeout",
          "value" : "600"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "oozie-OOZIE_SERVER-410863ccd3100e57b635ec541acb8d9d",
        "type" : "OOZIE_SERVER",
        "hostRef" : {
          "hostId" : "i-048ee553725f66843"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2t6nr1ypb4b5m2asoowbyq2xm"
          } ]
        }
      } ],
      "displayName" : "Oozie"
    }, {
      "name" : "yarn",
      "type" : "YARN",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "mapred_reduce_tasks",
            "value" : "2"
          }, {
            "name" : "mapred_submit_replication",
            "value" : "2"
          }, {
            "name" : "mapreduce_map_cpu_vcores",
            "value" : "2"
          }, {
            "name" : "mapreduce_map_java_opts_max_heap",
            "value" : "1717986918"
          }, {
            "name" : "mapreduce_map_memory_mb",
            "value" : "2048"
          }, {
            "name" : "mapreduce_reduce_java_opts_max_heap",
            "value" : "3435973837"
          }, {
            "name" : "mapreduce_reduce_memory_mb",
            "value" : "4096"
          } ]
        }, {
          "roleType" : "JOBHISTORY",
          "items" : [ {
            "name" : "mr2_jobhistory_java_heapsize",
            "value" : "593494016"
          } ]
        }, {
          "roleType" : "NODEMANAGER",
          "items" : [ {
            "name" : "yarn_nodemanager_heartbeat_interval_ms",
            "value" : "100"
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/yarn/nm"
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/yarn/container-logs"
          }, {
            "name" : "yarn_nodemanager_resource_cpu_vcores",
            "value" : "4"
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "3537"
          } ]
        }, {
          "roleType" : "RESOURCEMANAGER",
          "items" : [ {
            "name" : "resource_manager_java_heapsize",
            "value" : "593494016"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_mb",
            "value" : "4273"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_vcores",
            "value" : "3"
          } ]
        } ],
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "90"
        }, {
          "name" : "yarn_service_cgroups",
          "value" : "false"
        }, {
          "name" : "yarn_service_lce_always",
          "value" : "false"
        }, {
          "name" : "zk_authorization_secret_key",
          "value" : "RpamHF6i7UuCka9ZFyYeahJ2gd8wFQ"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "yarn-JOBHISTORY-410863ccd3100e57b635ec541acb8d9d",
        "type" : "JOBHISTORY",
        "hostRef" : {
          "hostId" : "i-048ee553725f66843"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "91pb6dhr89f1zldbmirzo7uub"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-0bef6295e924612353f8a8bd0c276f19",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-0a1da5f86407b0799"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "al7qugpwvkcxh5ief0wj2zaxh"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-7cce873b6e102ea67626e37de8acb787",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-09b9b81d5c51f2ce7"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "ck9oomdypmvzrxyl92iuyl31j"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-bcae5707b2963b28316034c1fd2dabf4",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-0cf9327bd671c8b3b"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "4gkgg9wwoaq3powwto8kjceac"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-c3b7a8e02b04a8dc19451f367409d9f6",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-07311d22df2d63466"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "3kxwb18xov0bc4hkpf7etwll3"
          } ]
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-410863ccd3100e57b635ec541acb8d9d",
        "type" : "RESOURCEMANAGER",
        "hostRef" : {
          "hostId" : "i-048ee553725f66843"
        },
        "config" : {
          "items" : [ {
            "name" : "rm_id",
            "value" : "53"
          }, {
            "name" : "role_jceks_password",
            "value" : "dnpli25wh4al8k2zya4e02b3s"
          } ]
        }
      } ],
      "displayName" : "YARN (MR2 Included)"
    }, {
      "name" : "hdfs",
      "type" : "HDFS",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "BALANCER",
          "items" : [ {
            "name" : "balancer_java_heapsize",
            "value" : "593494016"
          } ]
        }, {
          "roleType" : "DATANODE",
          "items" : [ {
            "name" : "dfs_data_dir_list",
            "value" : "/dfs/dn"
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "3219965132"
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "4294967296"
          }, {
            "name" : "dfs_datanode_use_datanode_hostname",
            "value" : "true"
          } ]
        }, {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "dfs_client_use_trash",
            "value" : "true"
          } ]
        }, {
          "roleType" : "JOURNALNODE",
          "items" : [ {
            "name" : "dfs_journalnode_edits_dir",
            "value" : "/var/log/cloudera/jn"
          } ]
        }, {
          "roleType" : "NAMENODE",
          "items" : [ {
            "name" : "dfs_name_dir_list",
            "value" : "/dfs/nn"
          }, {
            "name" : "dfs_namenode_servicerpc_address",
            "value" : "8022"
          } ]
        }, {
          "roleType" : "SECONDARYNAMENODE",
          "items" : [ {
            "name" : "fs_checkpoint_dir_list",
            "value" : "/dfs/snn"
          }, {
            "name" : "secondary_namenode_java_heapsize",
            "value" : "593494016"
          } ]
        } ],
        "items" : [ {
          "name" : "dfs_client_use_datanode_hostname",
          "value" : "true"
        }, {
          "name" : "dfs_ha_fencing_cloudera_manager_secret_key",
          "value" : "4CKA1dVsnvTPP5eWAyjbbNN0UD2MWx"
        }, {
          "name" : "dfs_ha_fencing_methods",
          "value" : "shell(true)"
        }, {
          "name" : "fc_authorization_secret_key",
          "value" : "pH36zgtEE7cOU2sSL2oUnhSHY5qJHF"
        }, {
          "name" : "http_auth_signature_secret",
          "value" : "2I972JoXt1rIg1Hl1Jqk1n2b24Vc4q"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "10"
        }, {
          "name" : "service_health_suppression_hdfs_ha_namenode_health",
          "value" : "true"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hdfs-BALANCER-410863ccd3100e57b635ec541acb8d9d",
        "type" : "BALANCER",
        "hostRef" : {
          "hostId" : "i-048ee553725f66843"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-DATANODE-0bef6295e924612353f8a8bd0c276f19",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-0a1da5f86407b0799"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "7rt5kp525l29gspggn94t5viy"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-7cce873b6e102ea67626e37de8acb787",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-09b9b81d5c51f2ce7"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1xkcv39cat2w7oujz3lrzw4y5"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-bcae5707b2963b28316034c1fd2dabf4",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-0cf9327bd671c8b3b"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "4wtw4ihb39c8mt4k50dbgko1t"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-c3b7a8e02b04a8dc19451f367409d9f6",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-07311d22df2d63466"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1ymn3uxfhgnsp1c5vmu0rytf6"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-410863ccd3100e57b635ec541acb8d9d",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "i-048ee553725f66843"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8b9vglfm1on65uzup47ssewfj"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-c3b7a8e02b04a8dc19451f367409d9f6",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "i-07311d22df2d63466"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "abq0kyyislashgivy3gpaslgi"
          } ]
        }
      }, {
        "name" : "hdfs-HTTPFS-410863ccd3100e57b635ec541acb8d9d",
        "type" : "HTTPFS",
        "hostRef" : {
          "hostId" : "i-048ee553725f66843"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "30zw9modaiixck5ue271mw1ys"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-0bef6295e924612353f8a8bd0c276f19",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "i-0a1da5f86407b0799"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2i6o3zydagsakf00o0zmo2qki"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-7cce873b6e102ea67626e37de8acb787",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "i-09b9b81d5c51f2ce7"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "a85vyzb2vylzw76r93i0v1tkx"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-bcae5707b2963b28316034c1fd2dabf4",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "i-0cf9327bd671c8b3b"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "bx8my511ceo686o6posw42iw5"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-410863ccd3100e57b635ec541acb8d9d",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "i-048ee553725f66843"
        },
        "config" : {
          "items" : [ {
            "name" : "autofailover_enabled",
            "value" : "true"
          }, {
            "name" : "dfs_federation_namenode_nameservice",
            "value" : "nameservice1"
          }, {
            "name" : "dfs_namenode_quorum_journal_name",
            "value" : "nameservice1"
          }, {
            "name" : "namenode_id",
            "value" : "55"
          }, {
            "name" : "role_jceks_password",
            "value" : "d6sooisj6o4s1j8ueuunzr6np"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-c3b7a8e02b04a8dc19451f367409d9f6",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "i-07311d22df2d63466"
        },
        "config" : {
          "items" : [ {
            "name" : "autofailover_enabled",
            "value" : "true"
          }, {
            "name" : "dfs_federation_namenode_nameservice",
            "value" : "nameservice1"
          }, {
            "name" : "dfs_namenode_quorum_journal_name",
            "value" : "nameservice1"
          }, {
            "name" : "namenode_id",
            "value" : "69"
          }, {
            "name" : "role_jceks_password",
            "value" : "brd3x8b8aiwy3gxgc9z7ab8uy"
          } ]
        }
      } ],
      "displayName" : "HDFS"
    } ]
  } ],
  "hosts" : [ {
    "hostId" : "i-0cf9327bd671c8b3b",
    "ipAddress" : "172.31.3.123",
    "hostname" : "ec2-54-187-169-81.us-west-2.compute.amazonaws.com",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "i-048ee553725f66843",
    "ipAddress" : "172.31.0.164",
    "hostname" : "ec2-54-191-166-77.us-west-2.compute.amazonaws.com",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "i-09b9b81d5c51f2ce7",
    "ipAddress" : "172.31.12.132",
    "hostname" : "ec2-54-202-101-228.us-west-2.compute.amazonaws.com",
    "rackId" : "/default",
    "config" : {
      "items" : [ {
        "name" : "host_dns_resolution_enabled",
        "value" : "false"
      } ]
    }
  }, {
    "hostId" : "i-0a1da5f86407b0799",
    "ipAddress" : "172.31.10.234",
    "hostname" : "ec2-54-202-111-88.us-west-2.compute.amazonaws.com",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "i-07311d22df2d63466",
    "ipAddress" : "172.31.13.230",
    "hostname" : "ec2-54-202-126-186.us-west-2.compute.amazonaws.com",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  } ],
  "users" : [ {
    "name" : "__cloudera_internal_user__aaded3f3-d8f8-48f6-8f10-44d9837f9dd3",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "e189ed4fd48f842338e7cd466b7c2fd6542714c389434b9ecb8fdd463c9e4d93",
    "pwSalt" : 5469337946169456016,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-EVENTSERVER-410863ccd3100e57b635ec541acb8d9d",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "0b7ccb8c0c83b16bc4bb4384a8f920230b99d51d3e112475803fa278faa72015",
    "pwSalt" : -8778338626416717918,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-HOSTMONITOR-410863ccd3100e57b635ec541acb8d9d",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "eb9686c8da6fad3faa59ce5d84e0772076b8c03ab3a6bd6752e33b5d3f44e5d5",
    "pwSalt" : 8524172698952050057,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-REPORTSMANAGER-410863ccd3100e57b635ec541acb8d9d",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "11e1aadcf9c328e93f39337c38d27d893f9f642553baadabdcd27d49f8aec9fc",
    "pwSalt" : 3196832994930583685,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-SERVICEMONITOR-410863ccd3100e57b635ec541acb8d9d",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "e41ca98efe3298a17e47be11a4b314194a9c1ad7f252c5061647c520475b671c",
    "pwSalt" : -4870586604619770967,
    "pwLogin" : true
  }, {
    "name" : "admin",
    "roles" : [ "ROLE_LIMITED" ],
    "pwHash" : "0409bbdf8b9a9b4ba36e0db83a081e118037becaa85e38c6297f7f04873d641e",
    "pwSalt" : -3330769824942598415,
    "pwLogin" : true
  }, {
    "name" : "minotaur",
    "roles" : [ "ROLE_CONFIGURATOR" ],
    "pwHash" : "c09265923ce99ebde7609c0d2797ad6ae07974e6d5735f2f104cd3b209c09626",
    "pwSalt" : 6638621729997011803,
    "pwLogin" : true
  }, {
    "name" : "sebastiankramp",
    "roles" : [ "ROLE_ADMIN" ],
    "pwHash" : "958538e4bbdc067172101d57ccf022a92634599b28b4ddb9a4c182148e8f502e",
    "pwSalt" : -5346860390422740222,
    "pwLogin" : true
  } ],
  "versionInfo" : {
    "version" : "5.8.3",
    "buildUser" : "jenkins",
    "buildTimestamp" : "20161019-1013",
    "gitHash" : "518f0d6d44abc87bc392646e4369a20c8192b7cf",
    "snapshot" : false
  },
  "managementService" : {
    "name" : "mgmt",
    "type" : "MGMT",
    "config" : {
      "roleTypeConfigs" : [ {
        "roleType" : "EVENTSERVER",
        "items" : [ {
          "name" : "event_server_heapsize",
          "value" : "593494016"
        } ]
      }, {
        "roleType" : "HOSTMONITOR",
        "items" : [ {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "1610612736"
        } ]
      }, {
        "roleType" : "REPORTSMANAGER",
        "items" : [ {
          "name" : "headlamp_database_host",
          "value" : "ip-172-31-0-164.eu-central-1.compute.internal"
        }, {
          "name" : "headlamp_database_name",
          "value" : "rm"
        }, {
          "name" : "headlamp_database_password",
          "value" : "cloudera"
        }, {
          "name" : "headlamp_database_user",
          "value" : "root"
        }, {
          "name" : "headlamp_heapsize",
          "value" : "593494016"
        } ]
      }, {
        "roleType" : "SERVICEMONITOR",
        "items" : [ {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "1610612736"
        } ]
      } ],
      "items" : [ ]
    },
    "roles" : [ {
      "name" : "mgmt-ALERTPUBLISHER-410863ccd3100e57b635ec541acb8d9d",
      "type" : "ALERTPUBLISHER",
      "hostRef" : {
        "hostId" : "i-048ee553725f66843"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "38kfidnzjj6i7o4nhizoi5iy7"
        } ]
      }
    }, {
      "name" : "mgmt-EVENTSERVER-410863ccd3100e57b635ec541acb8d9d",
      "type" : "EVENTSERVER",
      "hostRef" : {
        "hostId" : "i-048ee553725f66843"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "92l3pak7v9bbxz36aelsmolc0"
        } ]
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-410863ccd3100e57b635ec541acb8d9d",
      "type" : "HOSTMONITOR",
      "hostRef" : {
        "hostId" : "i-048ee553725f66843"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "ehcublrt8rfcyj8aidtl98a4f"
        } ]
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-410863ccd3100e57b635ec541acb8d9d",
      "type" : "REPORTSMANAGER",
      "hostRef" : {
        "hostId" : "i-048ee553725f66843"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "9ywa4ol70khi61tag7qkbqhb2"
        } ]
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-410863ccd3100e57b635ec541acb8d9d",
      "type" : "SERVICEMONITOR",
      "hostRef" : {
        "hostId" : "i-048ee553725f66843"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "3fd7zktv0nla9jx4sfm7d5fwb"
        } ]
      }
    } ],
    "displayName" : "Cloudera Management Service"
  },
  "managerSettings" : {
    "items" : [ {
      "name" : "CLUSTER_STATS_START",
      "value" : "10/24/2012 5:10"
    }, {
      "name" : "PUBLIC_CLOUD_STATUS",
      "value" : "ON_PUBLIC_CLOUD"
    }, {
      "name" : "REMOTE_PARCEL_REPO_URLS",
      "value" : "https://archive.cloudera.com/cdh5/parcels/{latest_supported}/,https://archive.cloudera.com/cdh4/parcels/latest/,https://archive.cloudera.com/impala/parcels/latest/,https://archive.cloudera.com/search/parcels/latest/,https://archive.cloudera.com/accumulo/parcels/1.4/,https://archive.cloudera.com/accumulo-c5/parcels/latest/,https://archive.cloudera.com/kafka/parcels/latest/,https://archive.cloudera.com/navigator-keytrustee5/parcels/latest/,https://archive.cloudera.com/spark/parcels/latest/,https://archive.cloudera.com/sqoop-connectors/parcels/latest/"
    } ]
  }
}```