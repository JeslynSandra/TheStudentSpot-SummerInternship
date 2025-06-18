# TASK 1: Basic Vulnerability Scan Using Nmap 

## OBJECTIVE
The goal of this task was to use Nmap to run a simple vulnerability scan on my own computer. I wanted to find out which ports were open and get an idea of what services might be running on those ports. Also, I aimed to understand the possible security risks related to these open ports.

This was done as part of my Cybersecurity Internship with The Student Spot Summer Internship — May 2025.

---

## What is Nmap?  
From what I’ve learned, Nmap (short for Network Mapper) is a free tool that helps you see what devices and services are active on a network. It can detect IP addresses, MAC addresses, and hostnames of connected devices. More importantly, it helps identify potential weak spots like outdated software or open ports that hackers might target.

---

## TOOLS USED 
- Nmap version 7.97  
- Windows Command Prompt  
- Notepad  

---

## SYSTEM DETAILS  

| Parameter       | Value                   |
|-----------------|-------------------------|
| Operating System| Windows 10              |
| Nmap Version    | 7.97                    |
| Scan Type       | TCP Connect Scan (default) |
| Target          | localhost (127.0.0.1)   |

---

## COMMANDS I RAN  
I ran these commands in the Windows command prompt:

nmap localhost > scan_result.txt
notepad scan_result.txt

nmap -sV localhost > scan_result_det.txt
notepad scan_result_det.txt

## WHAT I DID
First, I ran a basic scan to see which TCP ports on my local machine were open. I saved the results to a file called scan_result.txt and opened it in Notepad to check the findings.

After that, I used the -sV option to get more detailed information about each open port, like the exact service running and its version number. This output went into scan_result_det.txt.

## SCAN RESULTS

| Port | State | Service       | Version              |
|------|-------|----------------|----------------------|
| 135  | open  | msrpc         | Microsoft Windows RPC |
| 445  | open  | microsoft-ds  | Unknown              |
| 3306 | open  | mysql         | MySQL 8.0.41         |
| 5432 | open  | postgresql    | PostgreSQL 9.6+      |

## FILES INCLUDED

- scan_result.txt – Basic Nmap scan output
- scan_result_det.txt – Detailed scan with service/version detection
- README.md – Full task documentation

## WHAT I LEARNED

Since I'm new to this field I didn’t realize how many services were actually open on my own system. Running the basic scan was useful, but using '-sV' gave me way more info — like version numbers that attackers could look up for known vulnerabilities. 

For example, seeing MySQL 8.0.41 and PostgreSQL running made me think about how exposed they might be if I were on a public or enterprise network.

Honestly, this task helped me see why network scans are step one in any security audit.



