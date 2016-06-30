```bash
ALLUXIO_JAVA_OPTS+="
    -Dalluxio.master.keytab.file=<YOUR_HDFS_KEYTAB_FILE_PATH>
    -Dalluxio.master.principal=hdfs/<_HOST>@<REALM>
    -Dalluxio.worker.keytab.file=<YOUR_HDFS_KEYTAB_FILE_PATH>
    -Dalluxio.worker.principal=hdfs/<_HOST>@<REALM>
    -Djava.security.krb5.realm=<YOUR_KERBEROS_REALM>
    -Djava.security.krb5.kdc=<YOUR_KERBEROS_KDC_ADDRESS>
"
```