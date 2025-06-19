# Task 3: Setting Up UFW Firewall on Ubuntu Virtual Machine

## Objective
Set up and configure a basic firewall using UFW (Uncomplicated Firewall) on an Ubuntu Linux virtual machine.

---

## VM Setup Process

### Download and Prepare Ubuntu VM
- Downloaded Ubuntu 24.04.2 Desktop ISO from [official mirror](https://mirror.ajl.albony.in/ubuntu-releases/24.04.2/ubuntu-24.04.2-desktop-amd64.iso).
- Created a new VM named "Ubuntu" in VirtualBox.
- Allocated 2048 MB RAM and 128 MB video memory.
- Mounted the ISO as a virtual optical drive.

### Installation Attempts & Troubleshooting
- Encountered issues including:
  - Virtual machine failing to boot due to missing OS or misconfigured boot order.
  - Black screen during boot caused by graphics incompatibilities.
  - Locked boot order settings in VirtualBox.
- Solutions applied:
  - Disabled EFI in VirtualBox settings.
  - Set boot order: Hard Disk first, Optical second.
  - Disabled 3D acceleration in Display settings.
  - Increased video memory to 128 MB.
  - Used GRUB menu `nomodeset` boot option to fix black screen.
  - Removed ISO from virtual drive after installation to enable boot from disk.

### Final Result
- Successfully installed Ubuntu 24.04.2 Desktop.
- VM boots to Ubuntu login screen without errors.

---

## UFW Firewall Installation and Configuration

### 1. Update package list
```bash
sudo apt update
```
2.Install UFW
```bash
sudo apt install ufw
```
3.sudo ufw status
```bash
sudo ufw status
```
4. Set default policies
```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```
5. Allow SSH 
```bash 
sudo ufw allow ssh
```
6. Enable UFW
```bash 
sudo ufw enable
```
7. Verify status
```bash
sudo ufw status verbose
```
What I Learned
This task taught me how to:

Set up and troubleshoot an Ubuntu VM in VirtualBox.

Solve boot and graphics issues by adjusting settings and boot options.

Install and configure a firewall using UFW to secure the system.

The importance of proper VM configuration and installation steps.


References
Ubuntu Official Installation Guide

UFW Documentation

VirtualBox community support and documentation






