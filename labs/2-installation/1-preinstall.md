* sudo vi /etc/sysctl.conf
  vm.swappiness=1
  check: cat /proc/sys/vm/swappiness

* df

* sysctl -a | grep hugepage

* sudo vi /etc/grub.conf
  append transparent_hugepage=never

* firewall
  sudo service iptables stop
  sudo chkconfig iptables off

* selinux
  check sestatus

* nscd
  sudo yum install nscd

* ntpd
  sudo yum install ntpd
  check timedatectl

* ulimit


* mariadb
  sudo yum install MariaDB-server MariaDB-client
  sudo systemctl start mariadb

* db-connector
  wget https://downloads.mariadb.com/Connectors/java/connector-java-2.0.2/
  export JAVA_HOME=/usr/bin/java/
  export CLASSPATH=/home/centos/mariadb-java-client-2.0.2.jar:$CLASSPATH

* mysql_secure_installation
