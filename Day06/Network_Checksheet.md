# Network Checksheet

## 📌 Install Net-Tools
```bash
sudo apt install net-tools  # Install net-tools on Ubuntu
```

---
## 🌐 Networking Basic Commands

| Command   | Description |
|-----------|-------------|
| ```ifconfig```  | Show or configure network interfaces |
| ```ip a```  | Display all network interfaces and their IPs |
| ```ip link```  | Show network interfaces without IP details |
| ```ip route```  | Show current routing table |
| ```netstat -rn```  | Display the kernel routing table |
| ```arp -a```  | View the ARP table |

---
## 🚀 Advanced Networking Commands

| Command   | Description |
|-----------|-------------|
| ```ip route add 192.168.1.0/24 via 192.168.1.1```  | Add a static route |
| ```ip rule show```  | Display routing rules |
| ```tc qdisc show```  | Show traffic control settings |
| ```brctl show```  | Show bridge information |
| ```ethtool eth0```  | Display Ethernet interface details |
| ```mtr google.com```  | Advanced traceroute with continuous output |

---
## 📊 Network Monitoring Commands

| Command   | Description |
|-----------|-------------|
| ```netstat -tulnp```  | Show all listening ports |
| ```ss -tulnp```  | Show open network sockets |
| ```tcpdump -i eth0```  | Capture network packets on eth0 |
| ```iftop```  | Monitor real-time bandwidth usage |
| ```nload```  | Show network traffic and usage |
| ```vnstat```  | Display historical network usage |

---
## 🏷️ DNS and Host Resolution Commands

| Command   | Description |
|-----------|-------------|
| ```nslookup google.com```  | Query DNS records for a domain |
| ```dig google.com```  | Get detailed DNS information |
| ```host google.com```  | Resolve a hostname to an IP |
| ```resolvectl status```  | Show DNS resolver status (systemd) |
| ```cat /etc/resolv.conf```  | View configured DNS servers |

---
## 🔗 Connectivity Commands

| Command   | Description |
|-----------|-------------|
| ```ping -c 4 google.com```  | Send 4 ICMP packets to test connectivity |
| ```traceroute google.com```  | Trace packet route to a destination |
| ```curl -I https://google.com```  | Fetch only HTTP headers |
| ```wget --spider https://google.com```  | Check URL availability |
| ```nc -zv google.com 443```  | Check if a specific port is open |

---
## 🔑 SSH and Remote Access Commands

| Command   | Description |
|-----------|-------------|
| ```ssh user@host```  | Connect to a remote system via SSH |
| ```scp file.txt user@host:/path```  | Copy a file to a remote system |
| ```rsync -avz file.txt user@host:/path```  | Sync files efficiently over SSH |
| ```ssh-keygen -t rsa -b 4096```  | Generate SSH keys |
| ```ssh-copy-id user@host```  | Copy SSH key to a remote server |
| ```ssh -L 8080:localhost:80 user@host```  | Create a local SSH tunnel |

---
## 🔐 Security Commands

| Command   | Description |
|-----------|-------------|
| ```ufw enable```  | Enable Uncomplicated Firewall (UFW) |
| ```ufw allow 22/tcp```  | Allow SSH traffic |
| ```iptables -L```  | List current firewall rules |
| ```fail2ban-client status```  | Check Fail2Ban service status |
| ```sudo lsof -i -P -n```  | List all open ports |
| ```chkrootkit```  | Scan for rootkits |
