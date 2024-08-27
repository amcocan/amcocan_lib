---
tags:
  - Post
  - Cybersecurity
  - FSO
---
___
# Vulnerability Analysis and Management
![[Vulnerability Management.jpeg]]
- [x] **What's the difference between Static Vulnerability Analysis vs. Dynamic Vulnerability Analysis? (update this post grammatically)**
- When talking about static and dynamic vulnerability analysis, all my research leads to static or dynamic code analysis specifically. In an article written by Harness, we can see the the differences between these two forms of vulnerability analysis by observing/comparing their individual benefits and understanding their specific use cases. Static code analysis (vulnerability analysis) performs vulnerability analysis on code without execution. This can identify issues early on in the development life cycle and offers a broad analysis of the codebase, but it lacks context related to runtime behavior and often returns false positives. Dynamic code analysis (vulnerability analysis) performs vulnerability analysis on code by running/executing the code. This shows how the code behaves in operating conditions and can offer deeper insights into behavioral issues like application logic, performance, and system interactions. However, this requires code to be executed and may miss any paths in the code (i.e., a feature in the code that was missed during testing/analysis) that are not executed during the vulnerability analysis. Given that both forms of vulnerability analysis have complementing benefits, I recommend that they be used together. Relying on just one can lead to undiscovered issues impacting business operations.
- [x] **What is the difference between Code Analysis vs. Vulnerability Management?**
- This question is a little easier to explain. Vulnerability management is comprised of multiple steps, out of which  code analysis is one. I fully addressed code analysis in the previous question, but I have yet to explain vulnerability management. According to the article by ServiceNow, vulnerability management consists of the following phases:
	1. Discover Vulnerabilities
	2. Prioritize Assets
	3. Assess Vulnerabilities
	4. Prioritize Vulnerabilities
	5. Remediate Vulnerabilities
	6. Verify Remediation
	7. Report on Status
- Code analysis is part of the first phase in vulnerability management known as the "Discovery" phase. Therefore, vulnerability management is a lifecycle consisting of multiple phases (6 - 7 depending on consolidation/approach) and code analysis is a part of the first phase in the vulnerability management lifecycle.
___
# Sources:

- Harness (2021, January 30). _Static vs. Dynamic Code Analysis: How to Choose Between Them_. Retrieved August 14, 2024, from https://www.harness.io/blog/static-vs-dynamic-code-analysis
- ServiceNow (n.d.). _What is vulnerability management?_ Retrieved August 14, 2024, from https://www.servicenow.com/products/security-operations/what-is-vulnerability-management.html
___