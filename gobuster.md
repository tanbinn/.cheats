# gobuster
% gobuster scanner

## gobuster - qucik_scan
#plateform/linux #target/remote #tag/scan
-b <状态码黑名单>
```bash
gobuster dir -u  <url> -w <dic> -b <StatusCode_blacklist> -t <threads_num> -x php,zip,bak,jpg,png,mp4,mkv,txt,html,md,git,7z,rar,db,log,docx,xlsx
```
