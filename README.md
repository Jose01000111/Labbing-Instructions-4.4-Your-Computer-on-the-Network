## 🧪 Labbing Instructions: 4.4 Your Computer on the Network (weight: 2)

---

>💬 **Tip:** Paste this study guide into ChatGPT and ask for **more instructions** by specifying:  
>- “Provide step-by-step lab instructions for this objective.”  
>- “Include which Linux distro to use (Debian/Ubuntu or RHEL/Fedora).”  
>- “Show examples of installing, verifying, and managing desktop and server applications.”  
>- “Include minimal command-line practice for package management and development tools.”  
>- “Focus only on what is most important for passing the LPI Linux Essentials exam.”  

>This will prompt ChatGPT to give **practical, exam-focused lab steps** for each section.

---

**Objective:** Explore and query network configuration, routing, DNS, and connectivity on a Linux system.

**Step-by-Step Lab Instructions:**

1. 🌐 **Check network interfaces and IP addresses**  
   - Command: `ip addr show`  
   - Observe: IP address (IPv4/IPv6), MAC address, interface status (UP/DOWN)  
   - Optional: `ifconfig` can also show interface info

2. 🚦 **Check routing table and default gateway**  
   - Command: `ip route show`  
   - Observe: Default gateway, routes to networks, interface association  
   - Optional: `route -n` for a numerical view

3. 🔧 **Monitor network connections and open ports**  
   - Command: `ss -tuln`  
   - Observe: Listening TCP/UDP ports, protocol type, local addresses  
   - Optional: `netstat -rn` to see routing info

4. 🧩 **Check DNS client configuration**  
   - Command: `cat /etc/resolv.conf`  
   - Observe: DNS server addresses  
   - Command: `cat /etc/hosts`  
   - Observe: Static hostname-to-IP mappings  

5. 🌍 **Test network connectivity**  
   - Command: `ping 8.8.8.8` — test raw connectivity to an IP  
   - Command: `ping google.com` — test DNS resolution and connectivity  

6. 🧩 **Query DNS records**  
   - Command: `host google.com`  
   - Observe: IP addresses returned for hostname, confirm DNS working

**Tips:**  
- Compare `ip addr show` and `ifconfig` outputs to understand different interface details.  
- Use `ss -tuln` to check if services are listening locally or remotely.  
- Observe differences between pinging an IP vs a hostname to see DNS resolution in action.  
- Modify `/etc/hosts` temporarily to test hostname mapping (exam concept).  
