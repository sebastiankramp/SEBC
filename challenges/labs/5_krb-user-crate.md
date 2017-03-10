##create user
```
kadmin.local -q "addprinc neymar"
kadmin.local -q "addprinc ronaldo"
kadmin.local -q "addprinc sloudera-scm"

```
##grand privileges

##generate keyfile
```
xst -k username.keytab hdfs/sk-node2@SEBASTIANKRAMP.ES
```