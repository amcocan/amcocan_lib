---
tags:
  - Post
  - FSO
  - Cybersecurity
---
___
## Instructions
**Replies** - due on **Thursday of Week 1**:
1. [x] Respond to at least one of your classmates.
2. [x] Comment on the article.  (25 word minimum)
3. [x] Do you agree with your classmate's interpretation of the events?  If so, why?  If not, why not?  (25 word minimum)
___
## Deven's Post
### [Snowflake Breach Exposes 165 Customers' Data in Ongoing Extortion Campaign](https://thehackernews.com/2024/06/snowflake-breach-exposes-165-customers.html)

**Summary:**
Snowflake's data breach impacted 165 customers due to compromised credentials purchased from cybercrime forums. The attack utilized information-stealing malware and involved systematic extortion by the UNC5537 threat actor. Measures are being taken to enhance security, including recommending multi-factor authentication (MFA).

**How does this article apply to Cybersecurity?**
The Snowflake breach highlights the ongoing threat of unauthorized access, data exfiltration, and information-stealing malware, emphasizing the importance of better security measures such as 2FA, endpoint protection solutions, and expiring login credentials.

**Did a GAP exist?**
Yes, The lack of 2FA and an endpoint protection solution to prevent data exfiltration introduced a gap for the threat actors to exploit, allowing them to steal customer information.

**Which Implementation Group (IG) applies to the entity?**
IG1 applies to the entity as it involves standard cybersecurity best practices that organizations should utilize such as implementation of 2FA and login credential management.

**Which CIS Controls should have been implemented by the entity?**
1. **CIS Control 3:** [**Data Protection**](https://www.cisecurity.org/controls/data-protection/)
   Develop processes and technical controls to identify, classify, securely handle, retain, and dispose of data.
2. **CIS Control 6:** [**Access Control Management**](https://www.cisecurity.org/controls/access-control-management/)
   Use processes and tools to create, assign, manage, and revoke access credentials and privileges for user, administrator, and service accounts for enterprise assets and software.
3. **CIS Control 10:** [**Malware Defenses**](https://www.cisecurity.org/controls/malware-defenses/)
   Prevent or control the installation, spread, and execution of malicious applications, code, or scripts on enterprise assets.
4. **CIS Control 13:** [**Network Monitoring and Defense**](https://www.cisecurity.org/controls/network-monitoring-and-defense/)
   Operate processes and tooling to establish and maintain comprehensive network monitoring and defense against security threats across the enterprise’s network infrastructure and user base.
5. **CIS Control 18:** [**Penetration Testing**](https://www.cisecurity.org/controls/penetration-testing/)
   Test the effectiveness and resiliency of enterprise assets through identifying and exploiting weaknesses in controls (people, processes, and technology), and simulating the objectives and actions of an attacker.

**Which of those controls were not implemented?**
CIS Control 10 and Control 13 were not implemented, the threat actor was able to utilize malware and filter out the stolen data from Snowflake’s system and network without it being detected until after the attack.
___
## Reply Post
**Hello Deven,**

Great choice for an article! Snowflake (a company that offers many cloud solutions such as cloud computing as a service) experienced a data breach recently that led to the compromise of client data. This article showcases a security GAP within Snowflake's system leading to your observations and suggestions on this article.

I agree with your interpretation of this article especially considering the security GAP that has been leveraged in the recent data breach. I believe that the CIS controls you listed are a great way for Snowflake to improve they security posture and mitigate GAP. Additionally, suggesting the application of Implementation Group 1 (IG1) to mitigate the existing GAP by offer basic cyber security measures such as Two-Factor Authentication (2FA) or Multi-Factor Authentication (MFA) was a great move. Overall, I found your post to be very informative and full of great suggestions with relation to Snowflake's recent data breach.
___