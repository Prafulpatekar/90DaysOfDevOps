# 🌍🚀 Essential Network Protocols & Ports for DevOps   

## 📌 **Overview**  
Networking plays a vital role in **DevOps, cloud computing, and CI/CD pipelines**. Understanding key **protocols and ports** is crucial for **security, infrastructure management, and troubleshooting**.   

---

## 🔥 **Key Network Protocols & Their Port Numbers**  

| 🌐 **Protocol** | 🔢 **Port Number(s)** | 📌 **Usage in DevOps & Cloud** |
|--------------|-----------------|-------------------------------|
| **HTTP** | 80 | Web applications, REST APIs, monitoring dashboards |
| **HTTPS** | 443 | Secure web traffic, SSL/TLS encryption |
| **SSH** | 22 | Secure remote access, Git authentication, server management |
| **FTP** | 21 | File transfer for deployment & backups |
| **SFTP** | 22 | Secure file transfer using SSH |
| **DNS** | 53 | Domain name resolution, Kubernetes service discovery |
| **SMTP** | 25, 587 | Sending automated emails from CI/CD pipelines |
| **IMAP/POP3** | 143, 110 | Fetching emails in monitoring systems |
| **MySQL** | 3306 | Database access for applications |
| **PostgreSQL** | 5432 | Database management for microservices |
| **MongoDB** | 27017 | NoSQL database used in cloud-based applications |
| **Redis** | 6379 | In-memory caching for high-speed apps |
| **RabbitMQ** | 5672 | Message queuing for distributed systems |
| **Elasticsearch** | 9200 | Log aggregation & full-text search (ELK stack) |
| **Kubernetes API** | 6443 | Managing Kubernetes clusters |
| **Docker API** | 2375, 2376 | Container management & orchestration |
| **NTP** | 123 | Time synchronization for distributed cloud systems |
| **VPN (OpenVPN, WireGuard)** | 1194, 51820 | Secure networking across cloud environments |
| **Grafana** | 3000 | Real-time monitoring dashboards |
| **Prometheus** | 9090 | Metrics collection for observability |
| **Consul** | 8500 | Service discovery and health checking |

---

## ⚙️ **How These Protocols Fit into DevOps Workflows?**  

🔹 **CI/CD Pipelines** → Relies on **SSH, HTTP, HTTPS, FTP** for code deployments.  
🔹 **Cloud & Infrastructure Management** → Uses **DNS, Kubernetes API, Docker API** for orchestration.  
🔹 **Microservices & Containerization** → Depends on **Redis, RabbitMQ, PostgreSQL, MongoDB** for scalability.  
🔹 **Monitoring & Logging** → Uses **Prometheus, Grafana, Elasticsearch, SMTP** for system observability.  
🔹 **Security & Access Control** → Requires **VPN, SFTP, TLS/SSL (HTTPS)** for encryption.  

---

## 🔒 **Best Practices for Managing Ports & Network Security**  

✅ **Limit Open Ports** → Only expose necessary services to reduce attack surfaces.  
✅ **Use Firewalls & Security Groups** → Define strict inbound & outbound rules.  
✅ **Enforce TLS/SSL (HTTPS, FTPS, SSH)** → Encrypt communication for security.  
✅ **Monitor Open Ports Regularly** → Prevent unauthorized access and vulnerabilities.  
✅ **Implement VPN & IAM Policies** → Restrict access to critical infrastructure.  
✅ **Container Networking Best Practices** → Avoid exposing internal services unnecessarily.  
✅ **Enable Logging & Auditing** → Track unusual traffic patterns with **AWS CloudTrail, VPC Flow Logs**.  

---

## 📖 **Further Reading & Resources**  

🔗 [Comprehensive TCP/IP Ports List](https://en.wikipedia.org/wiki/List_of_TCP_and_UDP_port_numbers)  
🔗 [IANA Port Number Registry](https://www.iana.org/assignments/service-names-port-numbers/service-names-port-numbers.xhtml)  
🔗 [Secure SSH Practices in DevOps](https://www.ssh.com/academy/ssh)  
🔗 [Kubernetes API Ports Explained](https://kubernetes.io/docs/reference/networking/)  
🔗 [Docker Networking Best Practices](https://docs.docker.com/network/)  
🔗 [AWS Security Groups & Network ACLs](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_SecurityGroups.html)  

---

✅ **Task Completed!** 🚀  

📌 **GitHub Repository:** [90 Days of DevOps - Networking](https://github.com/Prafulpatekar/90DaysOfDevOps/tree/master/2025/networking)  

💡 *Contributions are welcome! Open an issue or PR anytime.*  

🚀 **Happy DevOps Learning!** 🎉