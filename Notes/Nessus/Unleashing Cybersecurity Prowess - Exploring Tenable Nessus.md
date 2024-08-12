---
tags:
  - Tools
  - Notes
  - Reference
  - Resources
  - Cybersecurity
author: Danny Vargas
social: https://medium.com/@itdanny
Date: 2023-12-29
---
___
In today’s tutorial, we delve into the world of Tenable Nessus! Our blog is your go-to resource for understanding, mastering, and harnessing the power of Nessus, a cutting-edge vulnerability management tool. Join us on this journey as we unravel its multifaceted features, providing you with the knowledge and insights needed to fortify your digital defenses.

🔍 **Scalable Vulnerability Scanning:** Learn how Nessus empowers organizations of all sizes with its scalable and robust vulnerability scanning capabilities. From small businesses to enterprise-level networks, Nessus ensures comprehensive scans, identifying potential weaknesses that could be exploited by cyber threats.

🌐 **Network Discovery and Asset Identification:** Explore how Nessus excels in network discovery and asset identification. Discover every nook and cranny of your network, from devices to applications, ensuring that no potential vulnerability goes unnoticed. Nessus provides a comprehensive asset inventory, a crucial foundation for effective cybersecurity.

🛡️ **Advanced Compliance Auditing:** Dive into Nessus’ advanced compliance auditing features, designed to help organizations adhere to regulatory standards effortlessly. Stay ahead of compliance requirements and protect sensitive data with Nessus’ customizable audit policies and reporting capabilities.

🎯 **Precise Vulnerability Prioritization:** Uncover the art of vulnerability prioritization with Nessus. Understand how the tool categorizes and prioritizes vulnerabilities based on their severity, allowing you to focus your resources on fixing the most critical issues first. Maximize your cybersecurity efforts with targeted and efficient remediation strategies.

🚀 **Integration Capabilities:** Nessus can seamlessly integrate into an existing cybersecurity ecosystem. From ticketing systems to threat intelligence platforms, Nessus fosters collaboration and synergy, streamlining your security operations and response mechanisms.

🔐 **Continuous Monitoring and Assessment:** Explore the concept of continuous monitoring and assessment with Nessus. The tool goes beyond one-time scans, providing real-time insights into your network’s security posture. Nessus ensures that you are always in the know, ready to adapt to evolving cyber threats.

📈 **Performance Metrics and Reporting:** Delve into the world of performance metrics and reporting with Nessus. Uncover how the tool generates insightful reports, allowing you to track your cybersecurity progress, communicate findings to stakeholders, and demonstrate compliance to auditors.

Before I begin, I will need an activation code for the scanner. To do that, I will need to register with my email as shown in Figure 1.

![](https://miro.medium.com/v2/resize:fit:1400/1*goINWVehUisPgGx_j-lrmA.png)

Figure 1: Registration page

Once you have registered, Tenable will be sending you an email with your activation code and a link to download the scanner.

![](https://miro.medium.com/v2/resize:fit:1400/1*vaYLisTEaTn94kBGkfTyiQ.png)

Figure 2: Email with activation code.

> [!Note]
> Nessus Essentials vulnerability scanner has a limitation of 16 IP Addresses to scan, but for this tutorial it should be fine.

On the download page, there is a drop downs for Version and Platform. I will be using Nessus — 10.6.4 for Windows — x86_64. Tenable Nessus provides installers for the following platforms:

- Windows (32-bit and 64-bit)
- Linux (32-bit and 64-bit)
- Mac OS X (64-bit) I currently do not possess the Mac Silicon at this time to test on how it functions.

![](https://miro.medium.com/v2/resize:fit:1400/1*j8jgYrSB4oZhShPHQsKipQ.png)

Figure 3: Download Tenable Nessus
___
# Cloning VM

Tenable Nessus can be installed on your machine without Virtual Machine, but I prefer to install it on a Virtual Machine. Instead of doing a full clone, I will doing a linked clone as shown in Figure 4.
___
# Types of clones

### Full clones

Full clones are complete and independent copies of a virtual machine and operate separately from the original parent VM. Because they don’t share virtual disks with the original parent VM, full clones generally perform better than linked ones. However, they also take longer to create than linked clones. ‍

### Linked clones

A linked clone is a snapshot of a virtual machine that shares virtual disks with the parent VM in an on-going manner. This conserves disk space and allows multiple VMs to use the same software installation. Linked clones make it easier to create unique virtual machines for individual tasks. They are also easier to share among people who need access to the same virtual disks (like support and dev teams).

![](https://miro.medium.com/v2/resize:fit:1400/1*-pysrKpVPHm6wNUPdbgxKA.png)

Figure 4: VirtualBox — Linked Clone

### Installing Tenable Nessus

Now let’s start the new clone virtual machine. Once Windows 11 Enterprise has loaded, let’s start Nessus installation by double clicking the installer. Installation is simple just follow the prompts. The installer requires admin rights.

![](https://miro.medium.com/v2/resize:fit:1026/1*Vnc0q9YgCKQskboFDk3G9A.png)

Once the installer finishes, it should open your web browser. Click on the “**Connect via SSL**” button as shown in Figure 5. Note: The SSL certificate is self-signed, and it will display “**Your Connection isn’t private**”. To bypass that, click “**Advanced**” button and click on “**Continue to localhost (unsafe)**” link as shown in Figure 6.

![](https://miro.medium.com/v2/resize:fit:1400/1*EUfCS1sUT9BNgWRxZxihiQ.png)

Figure 5: Connect via SSL

![](https://miro.medium.com/v2/resize:fit:1400/1*_7XA9o-cw8oY7VGSJB6O2w.png)

Figure 6: Self Signed Certificate

Click “**Continue**” to proceed with the installation. Since the virtual machine is connected to the internet, Checking the checkbox is not required as shown in Figure 7.

![](https://miro.medium.com/v2/resize:fit:1400/1*-pTBtDP_jG5MfkyhqM3iRA.png)

Figure 7

Select the “**Register for Nessus Essentials**” option and click “**Continue**” as shown in Figure 8.

![](https://miro.medium.com/v2/resize:fit:1400/1*Y9GgNETAzZDNGkqkid2j_A.png)

Figure 8: Register for Nessus Essentials

Since I already have the activation code, I can go ahead and click “Skip” button as shown in Figure 9. If you do not have an activation code, proceed to fill in the required text boxes.

![](https://miro.medium.com/v2/resize:fit:1400/1*udJoJeMynTLJF27wYrVmWA.png)

Figure 9: Get activation code.

I am going to use the activation code that I got the email from Nessus. Once it is entered, press “Continue” button as shown .

![](https://miro.medium.com/v2/resize:fit:1400/1*Ydw-uL13egLFRABt2iJZyw.png)

Figure 10: Enter activation code.

Now let’s create a user account, enter a username and password as shown in Figure 11.

![](https://miro.medium.com/v2/resize:fit:1400/1*NqcYXlb6s5phELmJ1rwJuQ.png)

Figure 11: Create an account.

Nessus will now initialize and download the required plugin as shown in Figure 12. This will take a few minutes (~20 — 30 mins with a nvme drive).

![](https://miro.medium.com/v2/resize:fit:1400/1*RlaCTlVCUGBm6BgKIAjZYA.png)

Figure 12: Initializing Nessus

Once Nessus finishes initializing, it will go to the main page of the Nessus as shown in Figure 13. Before starting the scan, the plugins will need to compile first and do not worry, Nessus will perform this action for you automatically. Hover over the stat icon and it will show the percent which has been completed as shown in Figure 14. Again, this goes faster on a nvme drive compared to a mechanical drive.

![](https://miro.medium.com/v2/resize:fit:1400/1*4819xmI1QgHzfc3ZfG2smw.png)

Figure 13: Tenable Main Page

![](https://miro.medium.com/v2/resize:fit:1400/1*ZxhiKJVGPyjjhJswAJv5vg.png)

Figure 14: Compiling Plugins

This would be a great time to review [Tenable Research | Tenable®](https://www.tenable.com/research) while the plugins complies because it is going to be a while before it finishes. Tenable Research talks about Security Alerts, Zero-Day Research, Research Blogs, Webinars and Reports, and plus there is a community support as shown in Figure 15.

![](https://miro.medium.com/v2/resize:fit:1400/1*Vq5hhrR95Y-LTe4MnSi-2A.png)

Figure 15: Tenable Nessus Research.

Once the plugins are done compiling, click “**Settings**”. In the setting page, the Overview tab will provide the following information as shown in Figure 16:

- Version
- Licensed Hosts
- Last Updated
- License Expiration
- Plugin Set
- Policy Template Version
- Activation Code

The License Utilization, Software Update, Encryption Password, and Events tabs are self-explanatory.

![](https://miro.medium.com/v2/resize:fit:1400/1*TRvUpEdIipmjW1cNWryl7Q.png)

Figure 16: Overview tab

When click on “Scans” link for the first time, Tenable Nessus will open a dialog box with the following message. This is a getting started dialog which will perform a Host Discovery Scan.

> To get started, launch a host discovery scan to identify what hosts on your network are available to scan. Hosts that are discovered through a discovery scan do not count towards the 16 host limit on your license.
> 
> Enter targets as hostnames, IPv4 addresses, or IPv6 addresses. For IP addresses, you can use CIDR notation (e.g., 192.168.0.0/24), a range (e.g., 192.168.0.1–192.168.0.255), or a comma-separated list (e.g., 192.168.0.0, 192.168.0.1).

![](https://miro.medium.com/v2/resize:fit:1400/1*-xScfVwWDloqEyJ3r4-lKg.png)

Figure 17

![](https://miro.medium.com/v2/resize:fit:1400/1*5pg7h0ZJoaQTVMA0Y0A_Ig.png)

Figure 18

### Type of Scan Templates

Tenable Nessus stands out as a powerhouse in this arena, offering a versatile array of scanning templates to suit various needs. Let’s delve into some key templates and their roles in fortifying in security posture as shown in Figure 19.

![](https://miro.medium.com/v2/resize:fit:1400/1*KvuQ23tgM5ieKUVFFYacQg.png)

Figure 19: Scan templates
___
# Discovery Templates

### 1. Host Discovery

> Recommended Weekly

A simple yet effective scan to discover live hosts and open ports, providing valuable insights into your network’s composition. Tenable suggests running this scan weekly to stay abreast of new assets without impacting your license count.
___
# Vulnerability Templates

### 2. Basic Network Scan

Suitable for Any Host

A comprehensive system scan with all Nessus plugins enabled, ideal for internal vulnerability assessments across your organization’s systems.

### 3. Advanced Network Scan

Configurable to Any Policy

The most flexible scan type, allowing customization to match specific policies. Exercise caution with advanced templates to prevent misconfigurations that could lead to network saturation.

### 4. Advanced Dynamic Scan

Adaptable to New Plugins

An advanced scan with dynamic plugin filters, automatically incorporating new plugins released by Tenable. Tailor your scans for specific vulnerabilities while staying current.

### 5. Malware Scan

For Windows and Unix Systems

Utilizes a combined allow list and block list approach to detect malware, enhancing your organization’s security against potential threats.

### 6. Mobile Device Scan

>[!Note]
>This scan is not available with the free license.

Assess mobile devices via Microsoft Exchange or an MDM, scanning for installed applications and vulnerabilities. Ensure proper configuration for seamless scanning.

### 7. Credentialed Patch Audit

Authenticates Hosts and Enumerates Missing Updates

Directly accesses hosts to scan for missing patch updates, aiding in effective patch management.

### 8. Spectre and Meltdown

Remote and Local Checks

Identifies vulnerabilities related to Spectre and Meltdown, ensuring your systems are fortified against these critical threats.
___
# Threat Detection Templates

### 9. Ripple20 Remote Scan

Detects Treck Stack in the Network

Identifies hosts that may be affected by Ripple20 vulnerabilities, offering proactive threat detection.

### 10. Zerologon Remote Scan

Detects Microsoft Netlogon Vulnerability

Scans for the Zerologon vulnerability, a critical security check for Microsoft Netlogon.

### 11. Solarigate

Detects SolarWinds Solorigate Vulnerabilities

Utilizes both remote and local checks to identify vulnerabilities associated with SolarWinds Solorigate.

### 12. ProxyLogon: MS Exchange

Remote and Local Checks

Critical for Microsoft Exchange Server security, this template performs checks for specified CVEs, enhancing your defense against potential threats.

### 13. Log4Shell

Local and Remote Checks

Detects the Log4Shell vulnerability in Apache Log4j, an essential check for securing your systems against this critical issue.

### 14. CISA Alerts AA22–011A and AA22–047A

Remote and Local Checks

Aligns with CISA alerts AA22–011A and AA22–047A, providing thorough vulnerability assessments based on the latest alerts.

### 15. ContiLeaks

Remote and Local Checks

Ensures robust detection of vulnerabilities associated with ContiLeaks, a crucial aspect of defending against ransomware threats.

### 16. Ransomware Ecosystem

Remote and Local Checks

Comprehensive scanning for common ransomware vulnerabilities, enhancing your organization’s resilience against this pervasive threat.

### 17. 2022 Threat Landscape Retrospective (TLR)

Detects Vulnerabilities Featured in Tenable’s Report

Stay ahead of the curve by scanning for vulnerabilities highlighted in Tenable’s 2022 Threat Landscape Retrospective report.
___
# Compliance Templates

>[!Note]
>These templates are not available with the free license and will require an upgrade

### 18. Audit Cloud Infrastructure

Configuration Audits for Third-Party Cloud Services

Ensure the security of cloud services like AWS, Google Cloud, and Microsoft Azure by auditing their configurations regularly.

### 19. Internal PCI Network Scan

Meets PCI DSS 11.2.1 Requirements.

Satisfy internal PCI scanning requirements with this template, aiding in ongoing vulnerability management.

### 20. MDM Config Audit

Audits Mobile Device Managers

Enhance mobile device security by auditing configurations, including password requirements and usage of insecure features.

### 21. Offline Config Audit

Audits Network Device Configurations

For devices that don’t support secure remote access, perform offline configuration audits using host configuration files.

### 22. Unofficial PCI Quarterly External Scan

Simulates External Scans for PCI DSS Compliance

Simulate external scans to meet PCI DSS quarterly scanning requirements, though validation is limited to Tenable Vulnerability Management customers.

### 23. Policy Compliance Auditing

Audits System Configurations Against a Baseline

Ensure adherence to security policies by auditing system configurations against a known baseline.

### 24. SCAP and OVAL Auditing

Audits Systems Using SCAP and OVAL Definitions

Leverage NIST’s SCAP policies for managing vulnerabilities and policy compliance, with checks for both Linux and Windows systems.
___
# Demo

I have selected the Malware Scan template, and it will be scanning a Raspberry Pi 4 which has Ubuntu 22.04 currently installed. In the “**Basic**”, Enter the name and target. I will enter “**Rasp**” and IP address “**192.168.0.156**” as shown in Figure 20. I will leave the default configuration for Discovery, Assessment, Report, and Advance in the “**Settings**” tab.

![](https://miro.medium.com/v2/resize:fit:1400/1*4dF1qJV9PmoHmWzSNV8qJw.png)

Figure 20: Scan Options

On the “**Credentials**” tab, I will be logging in by **SSH**. In the SSH panel, change the Authentication method to “**password**” and enter the login credentials. In the “**Elevate Privileges with**” dropdown, select “**sudo**” and enter the “**sudo user**” and “**sudo password**” as shown in Figure 21.

![](https://miro.medium.com/v2/resize:fit:1400/1*U6b70CFqtwQ3U_joqxoxeQ.png)

Figure 21: Credentials

On the “**Plugins**” tab, it shows the plugins that the scanner will be using as shown in Figure 22. Clicking on the plugin will display more information as shown in Figure 23. Click “**save**” will save the configuration for this scan.

![](https://miro.medium.com/v2/resize:fit:1400/1*Beb2TFx_SvCUl3Z8vy4B7g.png)

Figure 22: Types of plugins

![](https://miro.medium.com/v2/resize:fit:1400/1*bykw6gPPZYBBvok8yjw1Zg.png)

Figure 23: Plugin information

On the side menu, click on “**My Scans**” and on the table it will show the newly created scan. Click on the “**play**” icon to start the scan as shown in Figure 24. This scan can take a few minutes to complete and once the scan is completed a check mark will appear on the Last Scanned column as shown in Figure 25. To review the results, click on the scan.

![](https://miro.medium.com/v2/resize:fit:1400/1*iWgv-bagr95iFkcPC-n0FQ.png)

Figure 24: My Scans

![](https://miro.medium.com/v2/resize:fit:1400/1*DZy7-QeKK36eLWDGus8-vQ.png)

Figure 25: Completed Scan

On the scan results page, I went ahead and clicked on the “**Vulnerabilities**” tab. As shown in Figure 26, the scan did not detect any Malware installed on the Raspberry Pi 4, but it did give us information about the device and label all the “**Severity**” as info. Selecting a row will display more information about the severity.

The Severity has a purpose, and this provides a Service Level Agreement (SLA) of when the vulnerability needs to be fixed. SLA is defined as

> “A Service Level Agreement (SLA) is a contractual agreement between a service provider and a customer that outlines the specific expectations, quality standards, and performance metrics for the services provided. SLAs serve as a crucial tool in defining the scope of services, establishing clear benchmarks, and ensuring accountability. They typically include details such as service availability, response times, resolution procedures, and any penalties or compensations for failing to meet agreed-upon standards. SLAs are vital in fostering transparency, managing expectations, and maintaining a mutually beneficial relationship between service providers and their clients.”

- **Critical —** 7 days
- **High** — 30 days
- **Medium** — 60 days
- **Low** — 180 days
- **Info** — N/A

>[!Note]
>These are the default date that Nessus provides.

![](https://miro.medium.com/v2/resize:fit:1400/1*4h3nxfrY7cW0phPkO94XUA.png)

Figure 26: Scan results

In Figure 27, it shows what the plugin was able to find. The plugin “**Microsoft Windows SMB shares Enumeration**” was able to detect the port and list the available SMB shares.

![](https://miro.medium.com/v2/resize:fit:1400/1*kNg_TrfD2HfGQ2JpLj051A.png)

Figure 27: Plugin Details
___
# Generating the Tenable Nessus Report

Generating the report is quite easy, Click the “**Report**” button and Generate Report dialog will appear. Select the following options and click “**Generate Report**”.

- Report Format: **HTML**
- Select a Report Template: **Detailed Vulnerabilities by Plugin**

![](https://miro.medium.com/v2/resize:fit:1400/1*ooM2ozFvGYMnY2XzAmC5Bw.png)

Figure 28: Generate Report Options

In Figure 29, The report shows all the Vulnerabilities by Plugin and along with Synopsis, Description, Solution, Risk Factor, Plugin Information, and Plugin Output.

![](https://miro.medium.com/v2/resize:fit:1400/1*AMyQH9bTo2zyeIcL9u5x5w.png)

Figure 29: Tenable Nessus HTML Report

In conclusion, whether you are safeguarding a small business or fortifying an enterprise-level network, Nessus proves to be an invaluable ally in the ongoing battle against cyber threats. This tutorial serves as a compass, guiding you through the intricate features of Tenable Nessus, equipping you with the knowledge and tools necessary to fortify, secure, and conquer the ever-evolving landscape of cybersecurity. Stay vigilant, stay informed, and let Tenable Nessus be your shield in the digital frontier. In the next tutorial, I will demonstrate on how to use the API that are built-in to Tenable Nessus.
___
# References

- Scan Templates. (n.d.). Retrieved from [https://docs.tenable.com/nessus/Content/ScanAndPolicyTemplates.htm](https://docs.tenable.com/nessus/Content/ScanAndPolicyTemplates.htm)
___