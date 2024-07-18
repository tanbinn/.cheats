# smbclient

% smbclient , file_svc
## smbclient - downalod_all_files
#plateform/linux #target/remote #tag/smb #port/445
字面意思。最好提前自己评估一下对面的大小
```bash
smbclient -c "recurse ON;prompt OFF;mget *" \\\\<ip>\\<volume> -U "<username>%<password>"
```

