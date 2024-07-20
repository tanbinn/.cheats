# ldapsearch

% ldap , scan
## ldapsearch - base with auth
#plateform/linux #target/remote #tag/ldap #port/389
arsenal的ldapsearch命令太老了，主要是-D参数分布不合理，这里专门再写一个也便于区分
```bash
ldapsearch -x -H ldap://<address> -D "<username>@<domain>" -w '<password>' -b 'DC=<domain>,DC=<path>'
```

