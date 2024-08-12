---
tags:
  - Post
  - FSO
  - Cybersecurity
---
___
# Instructions
**Initial Post** - due by **Tuesday of Week 1:**
1. Select an article related to a current cybersecurity situation, preferably one that speaks to one of this week's topics.  If that is not possible, any current cybersecurity situation article will suffice.
2. Post the following information:
	- [x] Title of the article
	- [x] Article link, set to open in a new tab, in the discussion area.
	- [x] Article summary (25 word minimum)
	- [x] How it applies. (25 word minimum)
	- [x] Answer the following items:
		- What steps could have been taken to prevent the situation? (25 word minimum)
		- What did they do right? (25 word minimum)
		- How will this impact cyber security or the info sec community? (25 word minimum)
3.  Be thorough in your responses.
___
## New OpenSSH Vulnerability Could Lead to RCE as Root on Linux Systems
###### [Article Link](https://thehackernews.com/2024/07/new-openssh-vulnerability-could-lead-to.html)
OpenSSH a popular and widely used SSH service/client. Yesterday an article highlighting a new vulnerability in OpenSSH was released on [The Hacker News](https://thehackernews.com/2024/07/new-openssh-vulnerability-could-lead-to.html) mentioning the reintroduction of an older vulnerability (a signal handler race condition) into `OpenSSH versions 8.5p1 to 9.7p1`. According to the article, attackers can exploit this vulnerability to carry out **"unauthenticated remote code execution (RCE) with root privileges in glibc-based Linux systems"**. [(Newsroom, 2024)](https://thehackernews.com/2024/07/new-openssh-vulnerability-could-lead-to.html "(Newsroom, 2024) The current CVE for this issue is [`CVE-2024-6387`](https://nvd.nist.gov/vuln/detail/CVE-2024-6387) and the older CVE is [`CVE-2006-5051`](https://nvd.nist.gov/vuln/detail/CVE-2006-5051). As of now, security updates to patch this vulnerability have been released by OpenSSH maintainers.

This article applies to our industry as it is our responsibility to secure networks and systems belonging to our employing organizations. Many times that means researching new Common Vulnerabilities and Exposures (CVEs) and implementing security updates or patches. We may also want to create strong policies for maintaining system dependencies or assets ensuring a more robust security posture.

One thing that the maintainers for OpenSSH could have done is analyze each release or update for the possible reintroduction of past vulnerabilities. Just because a vulnerability was patched does not mean that it can't be reintroduced during the development of a service. This requires a proactive approach and considerable amounts of testing before releasing an update.

OpenSSH maintainers addressed the discovered vulnerability in a timely manner providing security updates and patches. Addressing vulnerabilities quickly is an important step for vendors and maintainers; as many people, companies, or organizations rely on such services. In cases where vendors or maintainers do not address issues/vulnerabilities quickly, organizations may switch to a different service or build a custom solution as a replacement. Knowing the impact [`CVE-2024-6387`](https://nvd.nist.gov/vuln/detail/CVE-2024-6387) can have, OpenSSH maintainers correctly and efficiently responded to the situation.

The quick response from OpenSSH maintainers will impact the cybersecurity community in a positive way. The community will be able to mitigate the risk associated with [`CVE-2024-6387`](https://nvd.nist.gov/vuln/detail/CVE-2024-6387) and continue normal operations. In this manner there will be no loss of trust or disruption of organizational assets/systems due to the OpenSSH tool/service.
## Sources:
Newsroom (2024, July 1). _New OpenSSH Vulnerability Could Lead to RCE as Root on Linux Systems._ The Hacker News. Retrieved July 2, 2024, from [https://thehackernews.com/2024/07/new-openssh-vulnerability-could-lead-to.html](https://thehackernews.com/2024/07/new-openssh-vulnerability-could-lead-to.html "https://thehackernews.com/2024/07/new-openssh-vulnerability-could-lead-to.html")

NIST (2006, September 27). _CVE-2006-5051 Detail_. NATIONAL VULNERABILITY DATABASE. Retrieved July 2, 2024, from https://nvd.nist.gov/vuln/detail/CVE-2006-5051

NIST (2024, July 1). _CVE-2024-6387 Detail_. NATIONAL VULNERABILITY DATABASE. Retrieved July 2, 2024, from https://nvd.nist.gov/vuln/detail/CVE-2024-6387
___