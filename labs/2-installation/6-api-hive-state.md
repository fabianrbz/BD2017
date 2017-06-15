## check
 curl -u admin:admin 'http://52.29.27.22:7180/api/v1/clusters/fabianrbz/services/hive'

## start
 curl -X POST -u admin:admin 'http://52.29.27.22:7180/api/v1/clusters/fabianrbz/services/hive/commands/start'

## stop
 curl -X POST -u admin:admin 'http://52.29.27.22:7180/api/v1/clusters/fabianrbz/services/hive/commands/stop'
