# 📌 Hands-On with Networking Commands

## 🚀 Overview
Networking commands are essential for diagnosing, troubleshooting, and optimizing network connections. Below is a cheat sheet explaining the purpose and usage of key networking commands.

---

## 🔍 **Essential Networking Commands**

### 1️⃣ **Ping** - Check Network Connectivity
- Used to test the reachability of a host and measure round-trip time.
- Example:
  ```bash
  ping google.com
  ```
- Output:
![image](https://github.com/user-attachments/assets/8af88072-b08e-47d3-a5ae-1112b69d1f9f)

  
### 2️⃣ **Traceroute / Tracert** - Trace Packet Routes
- Shows the path packets take to reach a destination.
- Example:
  ```bash
  traceroute google.com  # Linux/macOS
  tracert google.com     # Windows
  ```
- Output:
![image](https://github.com/user-attachments/assets/17f8ba15-a321-4b79-8b77-7d57d74a7ea8)

  
### 3️⃣ **Netstat** - Display Network Statistics
- Shows active connections, listening ports, and routing tables.
- Example:
  ```bash
  netstat -an
  ```
- Output:
![image](https://github.com/user-attachments/assets/2aa29523-fa4b-43cf-9c37-b78476817d5a)

  
### 4️⃣ **Curl** - Make HTTP Requests
- Used to interact with URLs and APIs.
- Example:
  ```bash
  curl -I https://www.example.com
  ```
- Output:
![image](https://github.com/user-attachments/assets/fc1440e2-2a6d-4b55-a3aa-b5f3e3944919)

  
### 5️⃣ **Dig / Nslookup** - DNS Lookup
- Used to query DNS records and troubleshoot domain issues.
- Example:
  ```bash
  dig google.com  # Linux/macOS
  nslookup google.com  # Windows
  ```
- Output:
![image](https://github.com/user-attachments/assets/c663dc22-999d-41c0-aa7e-07f4fc4f4984)


---

## 🎯 **Cheat Sheet Summary**

| Command  | Purpose | Example |
|----------|---------|---------|
| `ping`   | Check connectivity | `ping google.com` |
| `traceroute` / `tracert` | Trace network path | `traceroute google.com` |
| `netstat` | Show network statistics | `netstat -an` |
| `curl` | Test HTTP requests | `curl -I example.com` |
| `dig` / `nslookup` | DNS lookup | `dig google.com` |

---

## 📚 **Additional Resources**

🔗 [Linux Networking Commands Guide](https://linuxize.com/post/linux-network-commands/)

🔗 [Netstat Usage](https://www.geeksforgeeks.org/netstat-command-in-linux-with-examples/)

🔗 [How to Use Curl](https://curl.se/docs/manual.html)

🔗 [Traceroute Explained](https://www.howtogeek.com/134132/how-to-use-traceroute-to-identify-network-problems/)

---

💪 **Task Completed!** 🚀

📌 **GitHub Repository:** [90 Days of DevOps - Networking]📌 (https://github.com/Prafulpatekar/90DaysOfDevOps/tree/master/2025/networking)  

🚀 **Happy Coding!** 🎉
