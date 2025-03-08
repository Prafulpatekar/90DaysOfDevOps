# **🐧 LINUX for DevOps:**
- **🖥️ Operating System (OS)**
- **💻 Client OS vs Server OS**
- **🐧 Linux OS**
- **⚙️ How Linux Works**
- [**📁 Important Directories in Root Directory**](UBUNTU_ROOT_DIR.md)
- [**⌨️ Commands to Practice**](LINUX_COMMANDS.md)
- [**🌐 NGINX Server**](NGINX.md)
- **👥 Users & Groups**
- **🔑 SSH**
- **📂 File Permissions**
- **🔍 Day-To-Day Life Scenario (awk, grep, sed, find)**
- **🌎 Networking**
- **🗄️ Volumes**
- **📜 Shell Scripts**

---

## **🖥️ Operating System (OS)**
### **What is OS?**  
- An **Operating System (OS)** is **system software** that manages **hardware resources**, provides essential services, and enables users to run applications. In **DevOps**, the OS plays a crucial role in **automating infrastructure**, managing servers, running containers, and deploying applications efficiently. 🚀

### **Types of OS:**  
There are two main types of OS: **Client OS** and **Server OS**.

#### **1️⃣ Client OS 💻**  
- A **Client OS** is designed for **end users** to perform tasks like **browsing, running applications, or gaming**. It focuses on **user experience, responsiveness, and application support** rather than handling heavy server loads.  
✅ **Examples:** Windows 10/11, macOS, Ubuntu Desktop  

#### **2️⃣ Server OS 🏢**  
- A **Server OS** is optimized to **manage, run, and serve multiple users, applications, and services**. It focuses on **stability, security, scalability, and resource management** for hosting **databases, web applications, and enterprise services**.  
✅ **Examples:** Windows Server 2022, Ubuntu Server, CentOS, Red Hat Enterprise Linux (RHEL)  

---

## **🐧 Linux OS**
### **🕰️ History of Linux: How It Was Created & Its Inspiration**  
#### **1️⃣ The Inspiration: UNIX (1969) 🏛️**  
- Before **Linux**, there was **UNIX**, created in **1969** at **AT&T’s Bell Labs** by **Ken Thompson, Dennis Ritchie, and others**.  
- **UNIX was multi-user & multitasking** but **proprietary and expensive**.  
- In **1983**, **Richard Stallman** started the **GNU Project** to create a **free UNIX-like OS**, but it lacked a **working kernel**.  

#### **2️⃣ Birth of Linux (1991) 🎓**  
- In **1991**, **Linus Torvalds**, a **Finnish computer science student**, wanted a **free and open-source OS** like UNIX but without licensing restrictions.  
- He started developing a **new kernel** as a **hobby project** and announced it on a **Usenet forum (comp.os.minix)**.  
- The first version, **Linux 0.01**, was released in **September 1991**.  

#### **3️⃣ Why Do We Need Linux? 🤔**  
✅ **Free & Open Source** – Unlike UNIX, Linux is **free to use and modify**.  
✅ **Stability & Security** – Strong **process management and user permissions** make it more secure.  
✅ **Scalability** – Used in **small devices (Raspberry Pi) to supercomputers**.  
✅ **Customization** – Different **distributions (Ubuntu, CentOS, Debian, etc.)** exist for different use cases.  
✅ **Cloud & DevOps Friendly** – Powers **servers, containers, and cloud platforms like AWS, GCP, and Azure**.  

---

### **🌍 Different Flavors of Linux:**
1️⃣ **Ubuntu** 🟠 – A **user-friendly, Debian-based** Linux distribution **popular for desktops, servers, and cloud environments**.  
2️⃣ **RHEL (Red Hat Enterprise Linux)** 🔴 – A **commercial Linux distribution by Red Hat**, known for **security, stability, and enterprise support**.  

---

## **⚙️ How Linux Works & Its Architecture 🏗️**  

🔷 Linux is a **multi-user, multitasking** operating system that **manages hardware and software resources efficiently**. It acts as an **interface** between the **user** and the **computer hardware**, ensuring smooth operation.  

### **🛠️ Linux Architecture**
1️⃣ **🖥️ Hardware Layer** – Includes **CPU, RAM, Disk, Network Devices**.  
2️⃣ **🧠 Kernel (Core of Linux)** – Manages **processes, memory, devices, and networking**.  
3️⃣ **📚 System Libraries (glibc, libc, etc.)** – Provide essential **APIs** for kernel interaction.  
4️⃣ **⌨️ Shell (Command Line Interface - CLI)** – Translates **user commands** for the OS.  
5️⃣ **📦 User Applications** – Includes **browsers, text editors, and DevOps tools (Docker, Kubernetes, Ansible, etc.)**.  

---

## **🔐 How Linux is Secure?**
### **Key Security Features of Linux 🛡️**  

1️⃣ **📂 File & Folder Permissions (Access Control)**  
- Every file and directory has **three types of permissions**:  
  - **User (Owner) 👤** – The person who created the file.  
  - **Group 👥** – A collection of users who share access.  
  - **Others 🌍** – Any other user on the system.  

2️⃣ **🔑 Root User & Least Privilege Model**  
- **Only the root user (superuser)** can modify critical system files.  
- Regular users have **limited permissions**, reducing accidental security breaches.  

3️⃣ **🛡️ SELinux & AppArmor (Mandatory Access Control)**  
- **SELinux (Security-Enhanced Linux)**: Prevents **unauthorized access** to system files.  
- **AppArmor**: Restricts programs based on predefined **security profiles**.  

4️⃣ **🚫 No Direct Executables in User Directories**  
- Unlike Windows, **Linux does not execute files** from `/home/user/Downloads` directly.  
- Files must be explicitly marked as **executable** (`chmod +x file.sh`).  

5️⃣ **🔐 Strong User Authentication**  
- Supports **password hashing, key-based authentication, and two-factor authentication (2FA)**.  
- **Example:** SSH keys (`id_rsa`, `id_rsa.pub`) for secure remote login.  

6️⃣ **🛡️ Firewall & Network Security**  
- **iptables / nftables**: Configure firewall rules.  
- **Fail2Ban**: Blocks repeated failed login attempts to prevent brute-force attacks.  

7️⃣ **⚡ Frequent Security Updates**  
- Open-source nature ensures **fast security patches**.  
- Package managers like **apt, dnf, and yum** help update software securely.  

---

### **🚀 Summary: Why Linux is a DevOps Engineer’s Best Friend?**  
✅ **Free & Open Source** 🆓  
✅ **Highly Secure** 🔐  
✅ **Scalable & Customizable** 🏗️  
✅ **Preferred for Servers & Cloud** ☁️  
✅ **Powerful CLI & Scripting Capabilities** ⌨️  

---
