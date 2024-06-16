# nmap
% nmap scanner

## nmap1 - tcp_explore
#plateform/linux #tag/scan
```bash
nmap -sT -p0- <ip> -oA nmapscan/ports ;ports=$(grep open ./nmapscan/ports.nmap | awk -F '/' '{print $1}' | paste -sd ',');echo $ports >> nmapscan/tcp_ports;
```

## nmap2 - udp_explore
#plateform/linux #tag/scan
```bash
nmap -sU -p0- <ip> -oA nmapscan/udp ;ports_udp=$(grep open ./nmapscan/udp.nmap | awk -F '/' '{print $1}' | paste -sd ',');echo $ports_udp >> nmapscan/udp_ports;
```

## nmap3 - tcp_detail
#plateform/linux #tag/scan
```bash
nmap -sT -sV -sC -O -p$ports <ip> -oA nmapscan/detail
```
