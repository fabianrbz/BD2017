{
  "timestamp" : "2017-06-14T20:17:21.034Z",
  "clusters" : [ {
    "name" : "fabianrbz",
    "version" : "CDH5",
    "services" : [ {
      "name" : "zookeeper",
      "type" : "ZOOKEEPER",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "SERVER",
          "items" : [ {
            "name" : "maxSessionTimeout",
            "value" : "60000"
          }, {
            "name" : "zookeeper_server_java_heapsize",
            "value" : "184549376"
          } ]
        } ],
        "items" : [ ]
      },
      "roles" : [ {
        "name" : "zookeeper-SERVER-b56cf8ed6f43706c5103869380ade6d7",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "i-07633f10ee87caf24"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2v5872wujeo483cchyfwe760u"
          }, {
            "name" : "serverId",
            "value" : "1"
          } ]
        }
      } ],
      "displayName" : "ZooKeeper"
    }, {
      "name" : "hdfs",
      "type" : "HDFS",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "BALANCER",
          "items" : [ {
            "name" : "balancer_java_heapsize",
            "value" : "184549376"
          } ]
        }, {
          "roleType" : "DATANODE",
          "items" : [ {
            "name" : "datanode_java_heapsize",
            "value" : "745537536"
          }, {
            "name" : "dfs_data_dir_list",
            "value" : "/dfs/dn"
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "10736126771"
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "969932800"
          } ]
        }, {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "dfs_client_use_trash",
            "value" : "true"
          } ]
        }, {
          "roleType" : "NAMENODE",
          "items" : [ {
            "name" : "dfs_name_dir_list",
            "value" : "/dfs/nn"
          }, {
            "name" : "dfs_namenode_servicerpc_address",
            "value" : "8022"
          }, {
            "name" : "namenode_java_heapsize",
            "value" : "184549376"
          } ]
        }, {
          "roleType" : "SECONDARYNAMENODE",
          "items" : [ {
            "name" : "fs_checkpoint_dir_list",
            "value" : "/dfs/snn"
          }, {
            "name" : "secondary_namenode_java_heapsize",
            "value" : "184549376"
          } ]
        } ],
        "items" : [ {
          "name" : "dfs_ha_fencing_cloudera_manager_secret_key",
          "value" : "cIsmGhrk0th42eeXTArF4Ah3CKVPbt"
        }, {
          "name" : "fc_authorization_secret_key",
          "value" : "lSFLmakMdkczB5Zktb9As2hGIKwpHE"
        }, {
          "name" : "http_auth_signature_secret",
          "value" : "f6SyvXMV9vpYEHOUPaUvzUjL30cCWO"
        }, {
          "name" : "rm_dirty",
          "value" : "true"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hdfs-BALANCER-b56cf8ed6f43706c5103869380ade6d7",
        "type" : "BALANCER",
        "hostRef" : {
          "hostId" : "i-07633f10ee87caf24"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-DATANODE-35701e333b653a24c8fbe40cd07ea200",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "53bc0cdb-82a8-4a3b-9874-a59cac26aa1d"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "5ywf2keh24i0sar3cguji5mfv"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-9894ebd8e55eb2514025dc5738aa793d",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-05644825f025f9dd1"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "3dx03zhrwn4fgd0tzm9ctucfk"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-a64db6be97fe4586fd46d41e410098f4",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-0dc30be77fff00bef"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "vkipjlobe2vt3omigj78a80h"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-b56cf8ed6f43706c5103869380ade6d7",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "i-07633f10ee87caf24"
        },
        "config" : {
          "items" : [ {
            "name" : "namenode_id",
            "value" : "54"
          }, {
            "name" : "role_jceks_password",
            "value" : "77wb93d8hsm954uod7wdwtlbp"
          } ]
        }
      }, {
        "name" : "hdfs-SECONDARYNAMENODE-b56cf8ed6f43706c5103869380ade6d7",
        "type" : "SECONDARYNAMENODE",
        "hostRef" : {
          "hostId" : "i-07633f10ee87caf24"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "egdhapkk74ei46pmgpwddehoy"
          } ]
        }
      } ],
      "displayName" : "HDFS"
    }, {
      "name" : "hbase",
      "type" : "HBASE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "MASTER",
          "items" : [ {
            "name" : "hbase_master_java_heapsize",
            "value" : "184549376"
          } ]
        }, {
          "roleType" : "REGIONSERVER",
          "items" : [ {
            "name" : "hbase_bucketcache_size",
            "value" : "925"
          }, {
            "name" : "hbase_regionserver_java_heapsize",
            "value" : "745537536"
          } ]
        } ],
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs"
        }, {
          "name" : "rm_dirty",
          "value" : "true"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hbase-MASTER-b56cf8ed6f43706c5103869380ade6d7",
        "type" : "MASTER",
        "hostRef" : {
          "hostId" : "i-07633f10ee87caf24"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6ufa1ztnlfixeqifm00cq2rch"
          } ]
        }
      }, {
        "name" : "hbase-REGIONSERVER-35701e333b653a24c8fbe40cd07ea200",
        "type" : "REGIONSERVER",
        "hostRef" : {
          "hostId" : "53bc0cdb-82a8-4a3b-9874-a59cac26aa1d"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "143n3rf1waaqe3et3nbyt1tbc"
          } ]
        }
      }, {
        "name" : "hbase-REGIONSERVER-9894ebd8e55eb2514025dc5738aa793d",
        "type" : "REGIONSERVER",
        "hostRef" : {
          "hostId" : "i-05644825f025f9dd1"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1q1n7bvy6fqlbzbwef0i2k888"
          } ]
        }
      }, {
        "name" : "hbase-REGIONSERVER-a64db6be97fe4586fd46d41e410098f4",
        "type" : "REGIONSERVER",
        "hostRef" : {
          "hostId" : "i-0dc30be77fff00bef"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "dunytlddtez1g6tqj0cfihrzy"
          } ]
        }
      } ],
      "displayName" : "HBase"
    }, {
      "name" : "yarn",
      "type" : "YARN",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "mapred_reduce_tasks",
            "value" : "3"
          }, {
            "name" : "mapred_submit_replication",
            "value" : "1"
          } ]
        }, {
          "roleType" : "JOBHISTORY",
          "items" : [ {
            "name" : "mr2_jobhistory_java_heapsize",
            "value" : "184549376"
          } ]
        }, {
          "roleType" : "NODEMANAGER",
          "items" : [ {
            "name" : "node_manager_java_heapsize",
            "value" : "745537536"
          }, {
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
            "value" : "2"
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "1024"
          } ]
        }, {
          "roleType" : "RESOURCEMANAGER",
          "items" : [ {
            "name" : "resource_manager_java_heapsize",
            "value" : "184549376"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_mb",
            "value" : "1024"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_vcores",
            "value" : "2"
          } ]
        } ],
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs"
        }, {
          "name" : "rm_dirty",
          "value" : "true"
        }, {
          "name" : "zk_authorization_secret_key",
          "value" : "JJ3fQyNnHVpcqXv410C1Z8snAU5QOU"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "yarn-JOBHISTORY-b56cf8ed6f43706c5103869380ade6d7",
        "type" : "JOBHISTORY",
        "hostRef" : {
          "hostId" : "i-07633f10ee87caf24"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "c50wa456m435t2tqjgjcntkto"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-35701e333b653a24c8fbe40cd07ea200",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "53bc0cdb-82a8-4a3b-9874-a59cac26aa1d"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2ds088913lxqidkoond5mnhhe"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-9894ebd8e55eb2514025dc5738aa793d",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-05644825f025f9dd1"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "bns6gs5j9jluvl46ab93wjd1z"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-a64db6be97fe4586fd46d41e410098f4",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-0dc30be77fff00bef"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "3pmx7x0sm0bzv6ok55d0pmzyq"
          } ]
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-b56cf8ed6f43706c5103869380ade6d7",
        "type" : "RESOURCEMANAGER",
        "hostRef" : {
          "hostId" : "i-07633f10ee87caf24"
        },
        "config" : {
          "items" : [ {
            "name" : "rm_id",
            "value" : "52"
          }, {
            "name" : "role_jceks_password",
            "value" : "dm8wo9w6tiko135aj0fpsdop7"
          } ]
        }
      } ],
      "displayName" : "YARN (MR2 Included)"
    }, {
      "name" : "hive",
      "type" : "HIVE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "HIVEMETASTORE",
          "items" : [ {
            "name" : "hive_metastore_java_heapsize",
            "value" : "184549376"
          } ]
        }, {
          "roleType" : "HIVESERVER2",
          "items" : [ {
            "name" : "hiveserver2_java_heapsize",
            "value" : "184549376"
          }, {
            "name" : "hiveserver2_spark_driver_memory",
            "value" : "966367641"
          }, {
            "name" : "hiveserver2_spark_executor_cores",
            "value" : "2"
          }, {
            "name" : "hiveserver2_spark_executor_memory",
            "value" : "912680550"
          }, {
            "name" : "hiveserver2_spark_yarn_driver_memory_overhead",
            "value" : "102"
          }, {
            "name" : "hiveserver2_spark_yarn_executor_memory_overhead",
            "value" : "153"
          } ]
        } ],
        "items" : [ {
          "name" : "hbase_service",
          "value" : "hbase"
        }, {
          "name" : "hive_metastore_database_host",
          "value" : "52.29.27.22"
        }, {
          "name" : "hive_metastore_database_password",
          "value" : "hive_password"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hive-GATEWAY-35701e333b653a24c8fbe40cd07ea200",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "53bc0cdb-82a8-4a3b-9874-a59cac26aa1d"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-9894ebd8e55eb2514025dc5738aa793d",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-05644825f025f9dd1"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-a64db6be97fe4586fd46d41e410098f4",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-0dc30be77fff00bef"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-b56cf8ed6f43706c5103869380ade6d7",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-07633f10ee87caf24"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-HIVEMETASTORE-b56cf8ed6f43706c5103869380ade6d7",
        "type" : "HIVEMETASTORE",
        "hostRef" : {
          "hostId" : "i-07633f10ee87caf24"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1w92b7jinvi39yapo2h00tfqt"
          } ]
        }
      }, {
        "name" : "hive-HIVESERVER2-b56cf8ed6f43706c5103869380ade6d7",
        "type" : "HIVESERVER2",
        "hostRef" : {
          "hostId" : "i-07633f10ee87caf24"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "9apthgopleipxec8ffsg05rxx"
          } ]
        }
      } ],
      "displayName" : "Hive"
    }, {
      "name" : "oozie",
      "type" : "OOZIE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "OOZIE_SERVER",
          "items" : [ {
            "name" : "oozie_database_host",
            "value" : "52.29.27.22"
          }, {
            "name" : "oozie_database_password",
            "value" : "oozie_password"
          }, {
            "name" : "oozie_database_type",
            "value" : "mysql"
          }, {
            "name" : "oozie_database_user",
            "value" : "oozie"
          }, {
            "name" : "oozie_java_heapsize",
            "value" : "184549376"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "oozie-OOZIE_SERVER-b56cf8ed6f43706c5103869380ade6d7",
        "type" : "OOZIE_SERVER",
        "hostRef" : {
          "hostId" : "i-07633f10ee87caf24"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "4rgqewbtr1y24o2jgmxjcc7du"
          } ]
        }
      } ],
      "displayName" : "Oozie"
    }, {
      "name" : "hue",
      "type" : "HUE",
      "config" : {
        "roleTypeConfigs" : [ ],
        "items" : [ {
          "name" : "database_host",
          "value" : "52.29.27.22"
        }, {
          "name" : "database_password",
          "value" : "hue_password"
        }, {
          "name" : "database_type",
          "value" : "mysql"
        }, {
          "name" : "hbase_service",
          "value" : "hbase"
        }, {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "hue_webhdfs",
          "value" : "hdfs-NAMENODE-b56cf8ed6f43706c5103869380ade6d7"
        }, {
          "name" : "oozie_service",
          "value" : "oozie"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hue-HUE_SERVER-b56cf8ed6f43706c5103869380ade6d7",
        "type" : "HUE_SERVER",
        "hostRef" : {
          "hostId" : "i-07633f10ee87caf24"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "4vvc8vhlgwtzylq6r0wi8nqcc"
          }, {
            "name" : "secret_key",
            "value" : "vrM3D9DuchXXMeMdVwKfaE8XT6q0gW"
          } ]
        }
      } ],
      "displayName" : "Hue"
    } ]
  } ],
  "hosts" : [ {
    "hostId" : "i-07633f10ee87caf24",
    "ipAddress" : "172.31.0.39",
    "hostname" : "ip-172-31-0-39.eu-central-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "i-0dc30be77fff00bef",
    "ipAddress" : "172.31.1.58",
    "hostname" : "ip-172-31-1-58.eu-central-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "53bc0cdb-82a8-4a3b-9874-a59cac26aa1d",
    "ipAddress" : "172.31.15.228",
    "hostname" : "ip-172-31-15-228.eu-central-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "i-05644825f025f9dd1",
    "ipAddress" : "172.31.9.123",
    "hostname" : "ip-172-31-9-123.eu-central-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  } ],
  "users" : [ {
    "name" : "__cloudera_internal_user__mgmt-EVENTSERVER-b56cf8ed6f43706c5103869380ade6d7",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "7477e40f4455707189af61529dcf0c0868a3de00f1df689d8f1b5578ce1e964e",
    "pwSalt" : 1705880247730469620,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-HOSTMONITOR-b56cf8ed6f43706c5103869380ade6d7",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "0570157629d7a53824b5dd34bea569d32345d8fcb007d67a815da04ce7cae076",
    "pwSalt" : 1542803433457410619,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-REPORTSMANAGER-b56cf8ed6f43706c5103869380ade6d7",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "8a288c085f12073a80e67ca97202f4dbc8c35fa37ecc829209ae7674f04758ee",
    "pwSalt" : -6116289429229982035,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-SERVICEMONITOR-b56cf8ed6f43706c5103869380ade6d7",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "5bf2aee6db6fbecfb11b5486fbf5218a152bea01a4622d8abf332ef12961be87",
    "pwSalt" : -4145850445896503199,
    "pwLogin" : true
  }, {
    "name" : "admin",
    "roles" : [ "ROLE_ADMIN" ],
    "pwHash" : "72c85be6155d0e6b2294b7e55fb5130577687ba65ac08e077b7512015eee9b89",
    "pwSalt" : 2096369476522235970,
    "pwLogin" : true
  } ],
  "versionInfo" : {
    "version" : "5.11.1",
    "buildUser" : "jenkins",
    "buildTimestamp" : "20170525-1411",
    "gitHash" : "8adcfb8545cb0a35f590717b2626a9ea04948dae",
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
          "value" : "184549376"
        } ]
      }, {
        "roleType" : "HOSTMONITOR",
        "items" : [ {
          "name" : "firehose_heapsize",
          "value" : "268435456"
        }, {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "805306368"
        } ]
      }, {
        "roleType" : "REPORTSMANAGER",
        "items" : [ {
          "name" : "headlamp_database_host",
          "value" : "52.29.27.22"
        }, {
          "name" : "headlamp_database_name",
          "value" : "rman"
        }, {
          "name" : "headlamp_database_password",
          "value" : "rman_password"
        }, {
          "name" : "headlamp_database_user",
          "value" : "rman"
        }, {
          "name" : "headlamp_heapsize",
          "value" : "268435456"
        } ]
      }, {
        "roleType" : "SERVICEMONITOR",
        "items" : [ {
          "name" : "firehose_heapsize",
          "value" : "268435456"
        }, {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "805306368"
        } ]
      } ],
      "items" : [ ]
    },
    "roles" : [ {
      "name" : "mgmt-ALERTPUBLISHER-b56cf8ed6f43706c5103869380ade6d7",
      "type" : "ALERTPUBLISHER",
      "hostRef" : {
        "hostId" : "i-07633f10ee87caf24"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "akug4svuzu1aspkqul59w4a6a"
        } ]
      }
    }, {
      "name" : "mgmt-EVENTSERVER-b56cf8ed6f43706c5103869380ade6d7",
      "type" : "EVENTSERVER",
      "hostRef" : {
        "hostId" : "i-07633f10ee87caf24"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "ag57jsqcviymkjzzjz6jtenor"
        } ]
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-b56cf8ed6f43706c5103869380ade6d7",
      "type" : "HOSTMONITOR",
      "hostRef" : {
        "hostId" : "i-07633f10ee87caf24"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "enn05wcme5gcrcbzv9mcxb4du"
        } ]
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-b56cf8ed6f43706c5103869380ade6d7",
      "type" : "REPORTSMANAGER",
      "hostRef" : {
        "hostId" : "i-07633f10ee87caf24"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "aaijjlnin0wsacwfp0mvsr52u"
        } ]
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-b56cf8ed6f43706c5103869380ade6d7",
      "type" : "SERVICEMONITOR",
      "hostRef" : {
        "hostId" : "i-07633f10ee87caf24"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "3ehtuq2fiy7gatabbqhbxon2b"
        } ]
      }
    } ],
    "displayName" : "Cloudera Management Service"
  },
  "managerSettings" : {
    "items" : [ {
      "name" : "CLUSTER_STATS_START",
      "value" : "10/24/2012 14:00"
    }, {
      "name" : "PUBLIC_CLOUD_STATUS",
      "value" : "ON_PUBLIC_CLOUD"
    }, {
      "name" : "REMOTE_PARCEL_REPO_URLS",
      "value" : "https://archive.cloudera.com/cdh5/parcels/{latest_supported}/,https://archive.cloudera.com/cdh4/parcels/latest/,https://archive.cloudera.com/impala/parcels/latest/,https://archive.cloudera.com/search/parcels/latest/,https://archive.cloudera.com/accumulo/parcels/1.4/,https://archive.cloudera.com/accumulo-c5/parcels/latest/,https://archive.cloudera.com/kafka/parcels/latest/,https://archive.cloudera.com/navigator-keytrustee5/parcels/latest/,http://archive.cloudera.com/kudu/parcels/latest/,https://archive.cloudera.com/spark/parcels/latest/,https://archive.cloudera.com/sqoop-connectors/parcels/latest/"
    } ]
  }
}