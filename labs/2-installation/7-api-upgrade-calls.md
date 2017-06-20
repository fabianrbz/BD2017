curl -u admin:admin 'http://52.29.27.22:7180/api/version/'
  v14

curl -u admin:admin 'http://52.29.27.22:7180/api/v14/cm/version'
 {
     "version" : "5.9.2",
       "buildUser" : "jenkins",
         "buildTimestamp" : "20170330-1814",
           "gitHash" : "822da28bff818f57fc1bfc3eafe3a550300ef1b0",
             "snapshot" : false
 }

 curl -u admin:admin 'http://52.29.27.22:7180/api/v14/users'
   {
       "items" : [ {
             "name" : "admin",
                 "roles" : [ "ROLE_ADMIN" ]
                   } ]
   }

 curl -u admin:admin 'http://52.29.27.22:7180/api/v14/cm/scmDbInfo'
   {
       "scmDbType" : "MYSQL",
         "embeddedDbUsed" : false
   }
