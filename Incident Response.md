---
tags:
  - Cybersecurity
  - Notes
  - Formula
  - Tools
  - FSO
---
___
>[!Info] Incident Response
>It is the process by which an organization handles intrusion and cyberattacks.

| Terms         | Definitions                                                              |
| ------------- | ------------------------------------------------------------------------ |
| Vulnerability | A flaw or weakness in a system. (Compromises CIA)                        |
| Exploit       | A tool used to take advantage of a vulnerability.                        |
| Threat Actor  | An individual or agent (tools) that exploits vulnerabilities in systems. |
#### Incident Handling Process:
1. Preparation
2. Identification
3. Containment
4. Eradication
5. Recovery
6. Lessons Learned

>[!warning] Risk Formula: [CVE Score v3.0](https://nvd.nist.gov/vuln-metrics/cvss/v3-calculator)
>The **Base Score** is a function of the Impact and Exploitability sub score equations.
>**CVE Score** (`[AV/AC/PR/UI/S/C/I/A]`) = *Exploitability* (`AV/AC/PR/UI/S`) * *Impact* (`C/I/A`)

![[CVSS v3.1 Equations.png]]
#### Research Tools:
[National Vulnerability Database](https://nvd.nist.gov/)
[CVE Details](https://www.cvedetails.com/)
[ExploitDB](https://www.exploit-db.com/)
___