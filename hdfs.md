## Sorted space occupied
```
hdfs dfs -du "$1" | awk '{print $1,$2,$3}' | sort -nr | xargs -n3 sh -c 'printf "%s  %s  %s\n" $(numfmt --to=iec $0) $(numfmt --to=iec $1) $2'
```

##
command help
https://hadoop.apache.org/docs/stable/hadoop-project-dist/hadoop-common/FileSystemShell.html#count