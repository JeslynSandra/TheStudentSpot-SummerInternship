# TASK 2: OWASP Top 10 Web Vulnerabilities 

## Objective
To explore and understand the **OWASP Top 10** vulnerabilities that impact web applications, learn how to identify them, and study real-world examples of how they’ve been exploited.

This task was completed as part of my **Cybersecurity Internship** for The Student Spot Summer Internship – May 2025.


## Learnings about OWASP
OWASP, or the Open Worldwide Application Security Project, is best known for its Top 10 Web Vulnerabilities — a globally trusted list of the most critical risks in web applications. 
But it’s more than just a list. OWASP also offers free tools like OWASP ZAP to scan for website flaws, and tons of learning resources to help developers write secure code.
In short: OWASP is the guidebook to cybersecurity for anyone who is building/testing a web app.
The latest version (as of 2025) is the **OWASP Top 10 – 2021 Edition**.

## On What Basis Are The Vulnerabilities Identified?

- **Real-World Evidences**
  Most of the vulnerabilities come from the realistic intances which have happened over the years for a repeated period of time.OWASP digs into data from thousands of companies and hundreds of thousands of apps to spot the patterns. This info comes from security experts, firms, and big organizations around the globe, helping OWASP pick the most dangerous and common risks out there. 
- **Feedbacks and Opinions**
  A strong system comes from feedback — and OWASP knows that. They collect real-world data from thousands of apps and mix it with expert and community opinions to understand what actually causes harm. This helps them rank vulnerabilities not just by theory, but by how common, risky, and exploitable they really are.
- **Updation**
  OWASP doesn’t drop a new list every year — and that’s the point. They update the Top 10 roughly every 3 to 4 years, based on how much the threat landscape has actually changed. The goal isn’t to chase trends — it’s to reflect real-world data.


## OWASP Top 10 Vulnerabilities
The latest version as of 2025 is still the 2021 edition, and it introduced new categories like Insecure Design and Software Integrity Failures, which weren’t in older lists.

| # | Vulnerability                          | Description                                                                 | Real-World Example |
|---|----------------------------------------|-----------------------------------------------------------------------------|--------------------|
| 1 | **Broken Access Control**              | Users can access data/actions they shouldn’t.                              | In 2021, *Facebook* had a bug that let attackers access private posts. |
| 2 | **Cryptographic Failures**             | Sensitive data isn’t properly encrypted.                                   | *Adobe* stored millions of passwords with weak encryption during a 2013 breach. |
| 3 | **Injection**                          | Malicious input is used in queries/commands.                               | *Equifax* breach (2017) was caused by a command injection flaw. |
| 4 | **Insecure Design**                    | App lacks security measures during design phase.                           | No CAPTCHA/rate limit on login page allowed brute-force attacks. |
| 5 | **Security Misconfiguration**          | Default settings, verbose errors, or exposed files.                        | *NASA* exposed internal apps via an open Jenkins dashboard. |
| 6 | **Vulnerable and Outdated Components** | Outdated libraries or frameworks in use.                                   | The *Log4j* zero-day (2021) hit systems running old versions of Log4j. |
| 7 | **Identification & Authentication Failures** | Poor login/session management.                                          | *GitHub* had a session fixation bug allowing account hijack. |
| 8 | **Software & Data Integrity Failures** | Untrusted code/plugins loaded or unchecked updates.                        | *SolarWinds* supply chain attack (2020) compromised updates. |
| 9 | **Security Logging & Monitoring Failures** | No detection of suspicious behavior.                                  | *Capital One*’s logs failed to flag abnormal access patterns during their breach. |
| 10 | **Server-Side Request Forgery (SSRF)**| Server is tricked into making internal requests.                           | *Capital One* again — SSRF exposed AWS metadata via crafted URL. |


## What I Did  
I went through each vulnerability in the OWASP Top 10 – 2021 list using resources like OWASP.org and YouTube explainers — especially the Telusko channel, which really helped break things down in a simple way. I focused on what makes each flaw dangerous, how attackers take advantage of them, and looked up real-world examples to really get the full picture.


## What I Learned  
So basically, I learned how websites and apps can actually be exposed to breaches and unexpected risks — sometimes from small things like missing validation or bad config settings. Through this, I got a clear understanding of what OWASP stands for and how each of these vulnerabilities plays a role.

Knowing about these dangers makes you way more aware — not just to prevent attacks, but to respond smartly if something ever does go wrong. It’s like having a map before walking into a minefield.

## Files Included  
- `README.md` — Full documentation for Task 2  

