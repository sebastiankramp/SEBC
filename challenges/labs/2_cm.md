#list repos
```
ls /etc/yum.repos.d
cloudera-manager.repo  mysql-community.repo         redhat-rhui-client-config.repo
epel.repo              mysql-community-source.repo  redhat-rhui.repo
epel-testing.repo      redhat.repo                  rhui-load-balancers.conf

```
#scm-script
```
[root@ip-172-31-6-8 ec2-user]# /usr/share/cmf/schema/scm_prepare_database.sh mysql -h sk-node1 -utemp -ptemp --scm-host sk-node2 scm root cloudera
JAVA_HOME=/usr/java/jdk1.7.0_67-cloudera
Verifying that we can write to /etc/cloudera-scm-server
Creating SCM configuration file in /etc/cloudera-scm-server
Executing:  /usr/java/jdk1.7.0_67-cloudera/bin/java -cp /usr/share/java/mysql-connector-java.jar:/usr/share/java/oracle-connector-java.jar:/usr/share/cmf/schema/../liboudera.enterprise.dbutil.DbCommandExecutor /etc/cloudera-scm-server/db.properties com.cloudera.cmf.db.
[                          main] DbCommandExecutor              INFO  Successfully connected to database.
All done, your SCM database is configured correctly!

```