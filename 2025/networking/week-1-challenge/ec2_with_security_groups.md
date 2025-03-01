# ☁️ AWS EC2 & Security Groups

## 📌 Overview
Amazon Elastic Compute Cloud (EC2) is a scalable cloud computing service that allows users to deploy and manage virtual machines in the AWS Cloud. Security Groups serve as virtual firewalls, regulating inbound and outbound traffic to ensure secure access to instances.

---

## 🖥 **Launching an AWS EC2 Instance**

### ✅ Steps to Launch an EC2 Instance
1. **Log in to the AWS Management Console** → Search EC2 and click to open the EC2 Dashboard.
**PRO TIP** → Select Ireland Region for minimal cost.
2. **How to launch an instance** → Click "Launch Instance" and give a name or tag to your instance.
3. **Select OS/AMI** → Choose an Amazon Machine Image or Operating System Image like Ubuntu, Amazon Linux, Windows Server, if you are beginner select 'Free Tier Eligible' Image.
4. **Select an Instance Type Or Compute** → Choose an instance with required CPU, RAM, and storage. If you are beginner select 'Free Tier Eligible' Compute.
5. **Create or Select a Key Pair** → Generate a new key pair or can use an existing key-pair to access instance. A key pair to securely connect to your instance.
6. **Configure Network settings** → Select Firewall (Security groups) and Allow SSH traffic Anywhere.
7. **Configure Storage** → Enter storage GiB from 8 to 15 for Free tier.
8. **Launch the Instance** → Check the summary to ensure that you have entered 1 as the number of instances, then click on "Launch Instance." Once launched, wait for the instance status to change to "Running."
9. **Connect to the Instance** → Access the instance via SSH (Linux) or RDP (Windows).

### 🚀 Example: Connecting to an EC2 Instance via SSH
```sh
ssh -i path/to/key-pair.pem ec2-user@your-ec2-instance-public-ip
```
OR
```sh
ssh -i path/to/key-pair.pem public-ip-address
```

For Windows instances, use an RDP client to connect.

---

## 🔍 **Real-World Analogy**
- Think of **EC2 instances** as apartments within a gated community.
- **Security Groups** function like security guards controlling who can enter and exit.
- By setting up rules, you define which visitors (traffic) are allowed in or out for safety.


## 🔐 **Security Groups in AWS**

### ✅ What are Security Groups?
- Security Groups function as stateful virtual firewalls that control traffic at the **instance level**.
- Unlike Network ACLs (which operate at the subnet level), Security Groups evaluate **both inbound and outbound rules**.
- Each instance can have multiple Security Groups, and each Security Group can be assigned to multiple instances.


## 🔐 **Understanding AWS Security Groups**  

📌 **Security Groups** control inbound/outbound traffic based on rules. They act as **stateful firewalls**, allowing or denying access to EC2 instances.  

### **🔥 Inbound Rules (Incoming Traffic)**
| **Protocol** | **Port** | **Source** | **Purpose** |
|-------------|---------|-----------|-------------|
| **SSH**     | 22      | My IP     | Secure remote access |
| **HTTP**    | 80      | 0.0.0.0/0 | Web server access |
| **HTTPS**   | 443     | 0.0.0.0/0 | Secure web access |
| **MySQL**   | 3306    | Custom IP | Database connection (Limit to backend only) |
| **RDP**     | 3389    | Custom IP | Remote Desktop for Windows instances |
| **PostgreSQL** | 5432 | Custom IP | Database access |

### **🚀 Outbound Rules (Outgoing Traffic)**
By default, **all outbound traffic is allowed**.

---

## 🎯 **Best Practices for Security Groups**
💚 **Follow Least Privilege Principle** – Open only necessary ports.  

💚 **Restrict SSH (Port 22) Access** – Allow only **your IP** instead of `0.0.0.0/0`.  

💚 **Use IAM Roles for Permissions** – Instead of allowing public access. 
 
💚 **Monitor Traffic** – Enable **AWS CloudTrail & VPC Flow Logs**.  

💚 **Regularly Audit Security Groups** – Remove unused rules.  

💚 **Use Network ACLs** – For an additional layer of security.  

---

## 🔍 **How to Modify Security Groups?**
### **📌 Adding a New Rule**
1️⃣ Go to **AWS EC2 Dashboard → Security Groups**.  

2️⃣ Select the Security Group associated with your instance. 
 
3️⃣ Click on **Inbound Rules → Edit**.  

4️⃣ **Add a New Rule** (e.g., Allow **Port 443 for HTTPS**). 
 
5️⃣ Click **Save**.  

### **📌 Deleting Unused Rules**
- Identify **unused ports** and remove unnecessary access.  

---

## 📚 Additional Resources  

🔗 [AWS EC2 Documentation](https://docs.aws.amazon.com/ec2/)  

🔗 [Security Groups Best Practices](https://aws.amazon.com/premiumsupport/knowledge-center/ec2-security-group-best-practices/)  

🔗 [AWS Key Pair for SSH](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-key-pairs.html)  

🔗 [VPC Flow Logs](https://docs.aws.amazon.com/vpc/latest/userguide/flow-logs.html)  

🔗 [AWS Network ACLs](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-network-acls.html)  

---

💪 **Task Completed!** 🚀  

📌 **GitHub Repository:** [90 Days of DevOps - Network](https://github.com/Prafulpatekar/90DaysOfDevOps/tree/master/2025/networking)  
💡 *Contributions are welcome! Feel free to raise an issue or PR.*  

🚀 **Happy Coding!** 😍