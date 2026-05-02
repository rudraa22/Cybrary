# Nmap Commands Cheatsheet

Personal reference — Kanodiya Rudra | B.Sc. IT 6th Sem

---

## Host Discovery

| Command | Description |
|---|---|
| `nmap -sn 192.168.1.0/24` | Ping scan — find live hosts, no port scan |
| `nmap -Pn <target>` | Skip ping, treat host as up |
| `nmap -sL 192.168.1.0/24` | List targets only, no packets sent |
| `nmap --traceroute <target>` | Trace path to target |

## Port Scanning

| Command | Description |
|---|---|
| `nmap <target>` | Default — top 1000 TCP ports |
| `nmap -p 80,443,22 <target>` | Scan specific ports |
| `nmap -p- <target>` | Scan all 65535 ports |
| `nmap -F <target>` | Fast scan — top 100 ports only |

## Scan Types

| Command | Description |
|---|---|
| `nmap -sS <target>` | SYN stealth scan (needs root) |
| `nmap -sT <target>` | TCP connect scan (no root needed) |
| `nmap -sU <target>` | UDP scan |
| `nmap -sA <target>` | ACK scan — detect firewall rules |

## Service & OS Detection

| Command | Description |
|---|---|
| `nmap -sV <target>` | Detect service versions |
| `nmap -O <target>` | OS detection (needs root) |
| `nmap -A <target>` | Aggressive — OS + version + scripts + traceroute |

## NSE Scripts

| Command | Description |
|---|---|
| `nmap -sC <target>` | Run default scripts |
| `nmap --script vuln <target>` | Vulnerability detection |
| `nmap --script http-title <target>` | Grab HTTP page titles |
| `nmap --script banner <target>` | Grab service banners |

## Output & Speed

| Command | Description |
|---|---|
| `nmap -oN output.txt <target>` | Save as normal text |
| `nmap -oX output.xml <target>` | Save as XML |
| `nmap -T4 <target>` | Faster timing (T1–T5 scale) |
| `nmap -v <target>` | Verbose output |

---

> Only scan networks and systems you own or have explicit permission to test.
