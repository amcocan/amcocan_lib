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
## Malicious npm Packages Found Using Image Files to Hide Backdoor Code
**[Article Link](https://thehackernews.com/2024/07/malicious-npm-packages-found-using.html)**

Cybercriminals (Attackers) are getting smarter everyday and always find new methods to hide malicious code. From standard methods of obfuscation to more modern techniques, hiding malicious code to evade detection has given attackers an edge in compromising systems. Recently, some security researchers have found two malicious packages on the npm package registry that leveraged image files to conceal code for a backdoor and communication with a command-and-control (C2) server. The security team for npm took down those two packages, but not before they were downloaded a combined total of 238 times. [(Newsroom, 2024)](https://thehackernews.com/2024/07/malicious-npm-packages-found-using.html)

Given that the attackers can or have leveraged this attack to exfiltrate private data and establish unauthorized persistent access to systems, makes this case a cybersecurity and information security matter. As security professionals, using various tools and even manually vetting what opensource libraries we use is of critical importance. By expecting other service providers (hosts) to vet the libraries for us, we risk compromising our systems. In this case, the host (npm) is not held responsible if a company uses an unvetted opensource package that compromised their system. However, for the sake of security, reputation, and trust -- the npm security team took quick action and removed these malicious packages from their platform.

There are two big steps that I think could have mitigated this issue. The first is for the npm security team to try and develop stronger code scanning solutions to scan their packages before adding them to the platform (I am aware that npm has such solutions already in place). However, this is difficult to do especially since threat-actors always find new ways to avoid detection. The second solution is having everyone personally take the time to vet the open source packages they use and use the existing bug-bounty/reporting system to alert the npm security team of any malicious packages found. This is what happened, but I think that these packages could have been reported a lot sooner if everyone that use opensource packages would properly vet them beforehand. It is important to note that not all organizations/people will make a report or even vet opensource packages, so this can still be a hard issue to address.

I commend the researchers that reported their findings to the npm security team and the security team that took immediate action to remove the packages from their platform. This was the best way to handle the situation in my opinion. The npm security team responded quickly and efficiently understanding the severity of the issue. Likewise, the security researchers leveraged the communication channels established for reporting issues and concerns to inform npm of this issue.

I think that situations like this one will impact the security landscape from an awareness standpoint. Organizations might (should) start taking a more proactive security stance especially when vetting open source code/resources. Learning the importance of ensuring that you don't personally introduce vulnerabilities into your system due to negligence is of huge importance. This can help improve security strategies for organizations leading to an elevated standard of security on a national/global scale.
___
## Sources
Newsroom (2024, July 16). _Malicious npm Packages Found Using Image Files to Hide Backdoor Code_. The Hacker News. Retrieved July 16, 2024, from https://thehackernews.com/2024/07/malicious-npm-packages-found-using.html
___