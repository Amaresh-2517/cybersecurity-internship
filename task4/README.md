# Task 4 — Firewall Management on Kali Linux

## 🎯 Objective
Configure and manage firewall rules using **UFW (Uncomplicated Firewall)** on Kali Linux, including enabling, disabling, resetting, and uninstalling the firewall.

---

## 🛠 Environment
- **OS:** Kali Linux
- **Firewall Tool:** UFW (Uncomplicated Firewall)
- **Target Ports:** SSH (22), Telnet (23), HTTP (80), HTTPS (443)

---

## ⚡ Commands Used

### 1. Install UFW
```bash
sudo apt update
sudo apt install ufw -y


### Check status
sudo ufw status verbose

# Disable ufw
sudo ufw disable
sudo ufw status verbose

# Stop & disable auto-start
sudo systemctl stop ufw
sudo systemctl disable ufw

# (Optional) Mask ufw completely
sudo systemctl mask ufw

# Re-enable ufw if needed
sudo systemctl unmask ufw
sudo systemctl enable ufw
sudo systemctl start ufw

# Reset all rules
sudo ufw reset
sudo ufw status verbose

# Uninstall ufw
sudo apt remove --purge ufw -y
sudo apt autoremove -y



✅ Outcome :-
	•	Installed and verified UFW on Kali Linux.
	•	Configured inbound and outbound rules for SSH, HTTP, HTTPS, and Telnet.
	•	Practiced enabling, disabling, resetting, and removing firewall safely.
	•	Documented commands and troubleshooting steps for future reference.



❓ Interview Questions :-
	1.	What is a firewall?
    A security system that filters network traffic based on rules.
	2.	Difference between stateful and stateless firewall?
	•	Stateful: tracks active connections
	•	Stateless: filters packets individually
	3.	Inbound vs Outbound rules?
	•	Inbound: controls traffic coming into your system
	•	Outbound: controls traffic leaving your system
	4.	Why block Telnet (port 23)?
    Telnet is insecure and transmits data unencrypted.
	5.	How does a firewall improve security?
    Reduces attack surface and controls access to services.
	6.	What is NAT in firewalls?
    Network Address Translation hides private IPs and conserves public IPs.