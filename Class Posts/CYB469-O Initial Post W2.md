---
tags:
  - Post
  - FSO
  - Cybersecurity
---
___
## Instructions
**Initial Post** - due by **Tuesday**
1. Select an article related to a current cybersecurity situation, preferably one that speaks to one of this week's topics.  If that is not possible, any current cybersecurity situation article will suffice.
2. Post the following information:
	- [x] Title of the article
	- [x] Article link, set to open in a new tab, in the discussion area.
	- [x] Article summary (25 word minimum)
	- [x] How it applies (25 word minimum)
3. Answer the following items that apply.
	- [x] What steps could have been taken to prevent the situation? (25 word minimum)
	- [x] What did they do right? (25 word minimum)
	- [x] How will this impact cyber security or the info sec community? (25 word minimum)
4.  Be thorough in your responses.
___
## RADIUS Protocol Vulnerability Exposes Networks to MitM Attacks
[**Article link**](https://thehackernews.com/2024/07/radius-protocol-vulnerability-exposes.html)

This article covers a recent vulnerability found in the RADIUS network authentication protocol (known as BlastRADIUS), which can be exploited by an active-Man-in-the-Middle also known as a Mallory-in-the-Middle (MitM) attack. This vulnerability has been tracked as [CVE-2024-3596](https://nvd.nist.gov/vuln/detail/CVE-2024-3596) and has been given a CVSS score of 9.0. According to [a more detailed blog post](https://blog.cloudflare.com/radius-udp-vulnerable-md5-attack#:~:text=The%20attack%20allows%20a%20Monster%2Din%2Dthe%2DMiddle%20(MitM)%20with%20access%20to%20RADIUS%20traffic%20to%20gain%20unauthorized%20administrative%20access%20to%20devices%20using%20RADIUS%20for%20authentication%2C%20without%20needing%20to%20brute%20force%20or%20steal%20passwords%20or%20shared%20secrets.) on Cloudflare, "The attack allows a Monster-in-the-Middle (MitM) with access to RADIUS traffic to gain unauthorized administrative access to devices using RADIUS for authentication, without needing to brute force or steal passwords or shared secrets."

Such issues apply to the cybersecurity and information security, as it is our responsibility to secure systems and networks from bad actors. This is especially the case when taking into account the CVSS score assigned to [CVE-2024-3596](https://nvd.nist.gov/vuln/detail/CVE-2024-3596) and the risk of compromise to networks that rely on the RADIUS protocol.

One step that could have been taken to prevent this vulnerability is updating the cryptographic algorithm. The MD5 algorithm is known to be vulnerable to collision attacks. Replacing the outdated MD5 algorithm with stronger, more secure alternatives, would have prevented the possibility of collision attacks rendering this vulnerability obsolete. Well... maybe not 100% obsolete, but replacing the MD5 algorithm with stronger alternative would have substantially mitigated the issue.

One thing that has been done right is that short-term mitigation strategies have been developed quickly to deal with the vulnerability. Additionally, many vendors have released patches for this vulnerability. However, this is an issue that still requires attention from the developers for a long-term solution that can be used to mitigate this issue. That solution might take a while as properly implementing a new (stronger) cryptographic algorithm can take lots of time and testing.

This vulnerability can lead to many cyber-attacks on companies that use the RADIUS protocol in their network. These attacks can even lead to privilege escalation, data breaches, etc. Overall, this case can serve as an example for the whole industry on how using outdated or weak cryptographic algorithms increase risk. Organizations might even start looking deeper into external solutions they trust or use.
___
## Sources
Newsroom (2024, July 9). _RADIUS Protocol Vulnerability Exposes Networks to MitM Attacks_. The Hacker News. Retrieved July 9, 2024, from https://thehackernews.com/2024/07/radius-protocol-vulnerability-exposes.html

Cloudflare (2024, July 9). _RADIUS/UDP vulnerable to improved MD5 collision attack_. The Cloudflare Blog. Retrieved July 9, 2024, from https://blog.cloudflare.com/radius-udp-vulnerable-md5-attack
___