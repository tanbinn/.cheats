# feroxbuster

% feroxbuster scanner
#plateform/linux #target/remote #tag/scan

## feroxbuster - all_args 全要素自定义（仅参考）
```
feroxbuster -u <url> -H <标头> -x <指定想要扫描的文件后缀> -t <线程数，建议20> -w <字典路径>  --insecure --proxy <代理地址，如socks5h://127.0.0.1:9050> -C <指定想要的状态码> -N <筛选行数> -W <筛选字数> --rate-limit <限制每秒请求数> -d <最大递归深度>
```
## feroxbuster - quick_scan
```
feroxbuster -u <url> -t <线程数，建议20> -w <字典路径>  -C <指定想要的状态码>  -d <最大递归深度>
```

# gobuster
% gobuster scanner
#plateform/linux #target/remote #tag/scan

## gobuster - qucik_scan
```
gobuster dir -u  <url> -w <字典> -b <状态码黑名单> -t <线程数> -x php,zip,bak,jpg,png,mp4,mkv,txt,html
```
