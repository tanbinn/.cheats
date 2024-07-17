# crackmapexec

% cme , scanner , smb
## crackmapexec - smb explosion
#plateform/linux #target/remote #tag/explosion #port/445
用户爆破，需要用户名字典和密码字典。
```bash
crackmapexec smb <address> -u <username_file> -p <passwd_file> --continue-on-success --no-bruteforce
```
