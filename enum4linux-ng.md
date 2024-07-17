# enum4linux-ng

% enum4linux-ng , scanner
## enum4linux-ng - all_scan
#plateform/linux #target/remote #tag/scan #port/445
几乎全参数的扫描。
```bash
enum4linux-ng -A <ip> -C -oY <out_file>
```

## enum4linux-ng - scan_without_netbios
#plateform/linux #target/remote #tag/scan #port/445
相比-A参数，-As不会探测NetBIOS
```bash
enum4linux-ng -As <ip> -C -oY <out_file>
```

## enum4linux-ng - scan_login
#plateform/linux #target/remote #tag/scan #port/445
登录用户扫描
```bash
enum4linux-ng -A <ip> -C -u <username> -p "<password>" -oY <out_file>
```

