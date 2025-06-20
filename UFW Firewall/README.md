# Task 3: Firewall Configuration using firewalld (CentOS Stream 9)

## Objective
To set up and configure a basic firewall on a Linux virtual machine using `firewalld`, the default firewall management tool on CentOS.  
This task is part of the **Cybersecurity Internship** under **The Student Spot Summer Internship – May 2025**.

---

## Environment Details

| Parameter        | Value                     |
|------------------|---------------------------|
| Operating System | CentOS Stream 9 (64-bit)  |
| Virtual Machine  | VirtualBox                |
| Firewall Tool    | firewalld                 |
| Interface Used   | Terminal                  |

---

## Steps Performed

1. Installed `firewalld` (pre-installed on CentOS Stream 9).
2. Enabled and started the firewall service.
3. Verified that the firewall was active and running.
4. Set the default zone to `public`.
5. Allowed common services: **SSH**, **HTTP**, and **HTTPS**.
6. Opened a custom port: **8080/tcp**.
7. Verified that all services and ports were correctly added.
8. Removed **HTTP** as a test to practice rule management.
9. Reloaded the firewall and verified changes.

---

## 🔐 Commands Used

```bash
# This installs the firewall
sudo dnf install firewalld -y

# Enable and start the firewall service
sudo systemctl enable firewalld
sudo systemctl start firewalld

# Checks the state of the firewall
sudo firewall-cmd --state

# Add commonly used services
sudo firewall-cmd --permanent --add-service=ssh
sudo firewall-cmd --permanent --add-service=http
sudo firewall-cmd --permanent --add-service=https

# Open a custom port
sudo firewall-cmd --permanent --add-port=8080/tcp

# Reload to apply changes
sudo firewall-cmd --reload

# Check all current rules
sudo firewall-cmd --list-all

# Remove a service (as practice)
sudo firewall-cmd --permanent --remove-service=http
sudo firewall-cmd --reload
```
## Files Included
firewall-start-status.png – Shows successful enablement and active status of firewalld using systemctl status after installation. Confirms that the firewall is running and persistent.

firewall-enable–success.png -  Captures the full sequence of commands: installing firewalld, enabling and starting it, and verifying the status — all steps documented in one terminal session.

firewall-rules.png - Displays real-time firewall configuration: services (like SSH, HTTPS), custom port (8080/tcp) added, HTTP service removed, and --list-all outputs before and after reload.

firewalld-commands-log.txt – log of commands used 

## What I Learned
Before this, I had already explored some basic Linux commands in CentOS, but this task really helped me go deeper into how firewalls actually function. It wasn’t just about running a few commands — I got to understand what each service does, how to control access through ports, and why it matters in securing a system.

Getting hands-on with firewalld gave me a much clearer picture of how firewall rules are structured and applied in real time. Overall, it was a solid opportunity to move beyond theory and really grasp how Linux firewalls help keep systems safe.
