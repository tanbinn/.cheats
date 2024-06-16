# feroxbuster

% feroxbuster , scanner
## feroxbuster - all_args
#plateform/linux #target/remote #tag/scan
几乎全参数的扫描。实际情况中需要严格控制扫描频率。
```bash
feroxbuster -u <url> -H <head> -t <threads_num> -w <dic>  --insecure -C <Status_Code> --rate-limit <requests_per_seconds> -N <筛选行数> -W <筛选字数> -x <指定想要扫描的文件后缀> -d <depth> --proxy <代理地址，如socks5h://127.0.0.1:9050> 
```

## feroxbuster - quick_scan
#plateform/linux #target/remote #tag/scan
线程数，打靶场建议20以下，实战根据实际情况
-C <想要的状态码>
```bash
feroxbuster -u <url> -t <threads_num> -w <dic>  -C <Status_Code>  -d <depth>
```
