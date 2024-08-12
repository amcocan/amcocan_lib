---
tags:
  - Post
  - Cybersecurity
  - FSO
  - Tools
---
___
# CrowdStrike BSOD incident and how Wazuh avoids similar risks

- [x] **Provide a summary. In 100 words or more, Include why you choose this particular article.**
- Recently (as we are all aware) CrowdStrike was at the core of the "larges critical infrastructure blackout ever". Most Windows systems were hit with a BSOD loop as a result. This article briefly outlines that event and what Wazuh does differently to prevent such incidents from happening. One key difference between Wazuh and CrowdStrike **Extended Detection and Response (XDR)** is that Wazuh operates in the User Space rather than in the Kernel Space. Additionally, to safely interact with the operating system, Wazuh leverages standard kernel APIs to maximize compatibility and stability. The article proceeds to list some advantages of user space operations *(disadvantages were not listed, so be open minded)*. These advantages are enhanced stability, easier debugging due to simpler complexity, and improved security due to a limited access of the core operating system. Wazuh also pride themselves on being open sources and encouraging community collaboration, flexibility, and transparency.
- Overall, I chose to present this article or rather blog post, as it shows that there is more than one way to provide a solution. This should allow us to understand the importance of properly vetting any solution we choose to use. We must never blindly implement or rely on security tools without first understanding how they work and what the associated risks are. A bit part of our responsibilities as security specialists is ensuring that everything we use can be "trusted" and will not disrupt business continuity efforts. I hope that we can look at this article together and learn from previous incidents on how to better assess the risk of any tool/service we use.
___
# Sources:

- Wazuh (2024, July 19). _CrowdStrike BSOD incident and how Wazuh avoids similar risks_. Wazuh Blog. Retrieved August 8, 2024, from https://wazuh.com/blog/crowdstrike-bsod-incident-and-how-wazuh-avoids-similar-risks/
___