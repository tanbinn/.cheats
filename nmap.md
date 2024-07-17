# nmap
% nmap scanner

## nmap0 - ping_scan
#plateform/linux #tag/scan
```bash
nmap -sn <ip> -oA nmapscan/ip;ips=$(cat ./nmapscan/ip.nmap | grep -oP '(1\d{2}|2[0-4]\d|25[0-5]|[1-9]\d|[1-9])(\.(1\d{2}|2[0-4]\d|25[0-5]|[1-9]\d|\d)){3}');echo $ips >> ./nmapscan/ips_ping;
```

## nmap1 - tcp_explore
#plateform/linux #tag/scan
```bash
nmap -sT -p0- <ip> -oA nmapscan/ports ;ports=$(grep open ./nmapscan/ports.nmap | awk -F '/' '{print $1}' | paste -sd ',');echo $ports >> nmapscan/tcp_ports;
```

## nmap2 - udp_explore
#plateform/linux #tag/scan
```bash
nmap -sU -sS -T4 -p0- <ip> -oA nmapscan/udp ;ports_udp=$(grep open ./nmapscan/udp.nmap | awk -F '/' '{print $1}' | paste -sd ',');echo $ports_udp >> nmapscan/udp_ports;
```

## nmap3 - tcp_detail
#plateform/linux #tag/scan
```bash
nmap -sT -sV -sC -O -p$ports <ip> -oA nmapscan/detail
```
