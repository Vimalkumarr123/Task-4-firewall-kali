# 🔐 Task 4 – Firewall Configuration using UFW on Kali Linux

## 🎯 Objective
To configure and test basic firewall rules on Kali Linux using UFW (Uncomplicated Firewall). This task demonstrates how to control network traffic by blocking and allowing specific ports, thereby gaining basic firewall management skills.

---

## ⚙️ Tools & Environment
- **OS:** Kali Linux
- **Firewall:** UFW (Uncomplicated Firewall)
- **Terminal** for executing commands

---

## 🛠 Steps Executed

### 1. Check UFW Status
```bash
sudo ufw status

This command displays the current firewall status and any active rules.

2. Enable UFW

sudo ufw enable

Enables the firewall if it is not already active.

3. List Current Rules

sudo ufw status numbered

Shows a numbered list of existing firewall rules for easier management.

4. Block Inbound Traffic on Port 23 (Telnet)

sudo ufw deny 23

Blocks any incoming connection attempts on port 23, which is commonly used for Telnet.

5. Test the Block Rule

telnet localhost 23

When testing, the connection should fail (connection refused), confirming that port 23 is blocked.

6. Allow SSH on Port 22 (if accessing remotely)

sudo ufw allow 22

Ensures that SSH traffic (commonly used for remote access) is not blocked.

7. Remove the Test Block Rule (Optional)

sudo ufw delete deny 23

Deletes the rule blocking port 23 to restore the original state, if needed.

```
---

##📸 Evidence & Documentation

Command Log: A text file (firewall_steps.txt) containing all the executed commands and their outputs.

Summary: A brief description of how firewall rules work to filter network traffic based on defined rules.


---

##✅ Conclusion

This exercise provided hands-on experience in configuring a basic firewall using UFW on Kali Linux. Through this task, I learned how to:

Enable and configure UFW

Block and allow traffic on specific ports

Test firewall rules effectively


Task completed and documented for submission.
