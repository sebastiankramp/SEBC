#DB-Server

##Create Databases
```
mysql> create database scm;
Query OK, 1 row affected (0.01 sec)

mysql> create database rman;
Query OK, 1 row affected (0.00 sec)

mysql> create database hive;
Query OK, 1 row affected (0.00 sec)

mysql> create database oozie;
Query OK, 1 row affected (0.00 sec)

mysql> create database hue
    -> ;
Query OK, 1 row affected (0.00 sec)

mysql> create database sentry;
Query OK, 1 row affected (0.00 sec)

mysql>
```
##hostname
```
sk-node1
```
##Version
```

mysql> SELECT VERSION();
+-----------+
| VERSION() |
+-----------+
| 5.6.35    |
+-----------+
1 row in set (0.00 sec)

mysql>

```
##list databases
```

mysql> show databases;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| hive               |
| hue                |
| mysql              |
| oozie              |
| performance_schema |
| rman               |
| scm                |
| sentry             |
+--------------------+
9 rows in set (0.00 sec)

mysql>

```