# TheStudentSpot-SummerInternship

## Overview

This repository contains my completed tasks for the Cybersecurity Internship organized by The Student Spot.  
As someone new to cybersecurity, I joined this internship to gain practical skills in network security and system hardening. Each task challenged me to think like both a defender and an attacker, which deepened my understanding of real-world security practices.
---

## Tasks Completed

### Task 1: Basic Vulnerability Scan Using Nmap  
Performed TCP port scans on my local system using Nmap, identifying open ports and analyzing running services.  
Learned how to interpret scan results and the importance of service version detection in vulnerability assessment. 

Initially, I found interpreting the raw Nmap output confusing, especially understanding the significance of certain ports being open. It took me some time to correlate service versions with potential vulnerabilities. Using online resources and forums helped me develop a clearer understanding. This task reinforced the importance of reconnaissance in cybersecurity and made me appreciate how attackers gather information.

### Task 2: Understanding OWASP Top 10 Vulnerabilities  
Explored the OWASP Top 10 - 2021 edition vulnerabilities, their causes, and potential risks to web applications.  
Gained insights into secure coding practices and the importance of awareness in preventing common vulnerabilities.

### Task 3: Setting Up UFW Firewall on Ubuntu VM  
Set up a virtual machine with **CentOS Stream 9** and configured its built-in firewall tool `firewalld`.  
Enabled necessary services, opened a custom port, and practiced managing active firewall rules via the command line.  
Also gained experience troubleshooting VM setup issues and understanding the role of firewalls in securing Linux systems.
Setting up the VM and firewall was more challenging than expected. I initially struggled with service activation errors and port configuration mismatches. Through trial, error, and reading man pages, I gained confidence in using firewall commands and Linux system administration.

This task taught me that system hardening is a critical layer of defense and requires attention to detail and patience.

---

## Repository Structure

/Task-1-Nmap-Scan
├── scan_result.txt
├── scan_result_det.txt
└── README.md

/Task-2-OWASP-Top10
└── README.md

/Task-3-Firewall-CentOS
├── firewall-install-status.png
├── firewall-enable-status.png
├── firewall-rules.png
├── firewalld-commands-log.txt
└── README.md
