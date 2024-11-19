---
tags:
  - Cybersecurity
  - Notes
  - Certs
  - StudyGuide
  - Research
  - Resources
source: https://learning.oreilly.com/course/comptia-security-sy0-701/9780138251062/
updated: 2024-08-09T17:29:00
author: amcocan
---
___
# 1.1 Control Objectives

### Key Terms:

| Term:         | Definition:                                                                  |
| ------------- | ---------------------------------------------------------------------------- |
| Vulnerability | This is a weakness.                                                          |
| Threat        | This is a potential danger.                                                  |
| Threat Actor  | This is an adversary with malicious intent.                                  |
| Exploit       | This is when a threat actor successfully takes advantage of a vulnerability. |
### Controls:
**Controls** are *tactics*, *mechanisms*, and *strategies* that proactively minimize risk in one or more of the following ways.
- Reduce or eliminate a *vulnerability*.
- Reduce or eliminate the *likelihood* that a threat actor will be able to exploit a vulnerability.
- Reduce or eliminate the *impact* of an exploit.
> A control can do *one*, *two*, or all *three* of these -- but it **must** do at least one of these to be considered a control.
### Countermeasures:
**Countermeasures** are controls that are implemented to address a *specific* threat.
- Countermeasures are *generally reactive*.
- Countermeasures may be more effective, but *less efficient in a broad sense of application*.
### Trustworthy:
Controls should be verifiable (*trustworthy*).
- **Functionality:** What a control does.
- **Effectiveness:** How well a control works. This reflects the control's *consistent*, *complete*, *reliable*, and *timely* operation.
- **Assurance:** A measure of confidence that *intended* security controls are *effective* in their application.
### Control Objective:
A **Control Objective** is a statement of *desired results* or purpose to be achieved by implementing a control or set of controls. (**i.e.** What am I trying to achieve or accomplish?)
> *Control objective:* Protect hosts from malware infiltration.
> - Antivirus Software
> - Host Firewall
> - Restrict Email Attachments
> - URL Filtering
> - Sandboxing
### Security Control Diversity:
**Defense-In-Depth (layered security)** is the design and implementation of multiple overlapping layers of diverse controls.
- Controls should not be subject to a cascade effect and *should maintain independence*.
- *Diversity* of control type and associated vendor *should be considered*.
### Security Control Baselines:
**Security Control Baselines** express minimum standards for a given environment.
- Control baselines *serve as a starting point* and should be *strategically aligned with organizational needs*.
- Control baselines should be *proportionate to the criticality and sensitivity classification* of the asset being protected. (*Principle of proportionality*)
### Control Guidance:
- **NIST SP 800-53 Rev 5**
	- Security and privacy controls for information systems and organizations.
- **NIST Frameworks**
	- Cybersecurity Framework (CSF)
	- Privacy Framework
	- Risk Management Framework
- **ISO 27014:2020**
	- Information Security
	- Cybersecurity
	- Privacy Protection
### Fine-Tuning Controls:
- **Scoping**
	- Scoping is *eliminating unnecessary baseline recommendations* that are not applicable.
- **Tailoring**
	- Tailoring is *customizing baseline recommendations* to aline with organizational requirements.
- **Compensating**
	- Compensating is *substituting a recommended baseline* control with a similar one.
- **Supplementing**
	- Supplementing is *augmenting* (adding to) *the baseline recommendations*.
### Baseline Modification Process:
The following is the order for the baseline modification process.
1. **Identify Control Baseline**
2. **Apply Scoping Constraints**
3. **Tailor Controls**
4. **Select Compensating Controls** (If Needed)
5. **Supplement the Baseline** (If Needed)
6. **Publish**
7. **Implement**
8. **Assess**
9. **Monitor**
### Cost-Benefit Analysis:
Controls should be subject to a cost-benefit analysis.
> A **cost-benefit analysis** is the process of *comparing the estimated costs and benefits* to determine whether it makes sense to proceed from a business perspective.

| Key                               | Value                                                                             |
| --------------------------------- | --------------------------------------------------------------------------------- |
| Control Cost                      | The cost it takes to build, implement, and maintain the control.                  |
| Loss Cost                         | The cost of the losses without the control.                                       |
| Justified Cost                    | The cost of the control is justified.                                             |
| Unjustified Cost                  | The cost of the control is unjustified.                                           |
| Cost Justification (ROI Analysis) | An ROI analysis is required to determine the justification of the control's cost. |
```bash
Control Cost < Loss Cost == Justified Cost
Control Cost > Loss Cost == Unjustified Cost
Control Cost = Loss Cost == Cost Justification (ROI Analysis)
```
### Security-In-Action:
>[!question]+ Adopting a Control Baseline (CaseStudy)
External auditors have recommended that your organization adopt the **ISO 27014** as a control baseline. You concur with this recommendation. Management's response is that they worry about the applicability and cost of implementing such a broad control set. What could you say to them to alleviate their concerns?

>[!quote]+ Response (CaseStudy Solution)
>We may not implement all the controls in ISO 27014, but rather the ones that align with organizational needs. For that we will put the ISO 27014 publication through a *fine-tuning process* where we will subject it to *scoping*, *tailoring*, *compensating*, and *supplementing*. Additionally, we will conduct a *cost-benefit analysis* of the controls in ISO 27014 to ensure that implementing them make sense from a business perspective. (We can also ease the controls in slowly over time to prevent a large immediate expense)

___
# 1.2 Control Categories & Classifications
### Control Categories:
- **Technical**
	- Technical controls are *implemented using hardware, software, and/or firmware components*. Can be native or supplemental. (i.e., Firewalls, Cryptography, Authentication Systems, etc.)
- **Managerial**
	- Managerial controls *relate to risk management, governance, oversight, strategic alignment, and decision making*. (i.e., Risk Assessments, Project Management, etc.)
- **Operational**
	- Operational controls are *aligned with a process that is primarily implemented and executed by people*. (i.e., Change Management, Training, Testing, etc.)
- **Physical**
	- Physical controls are *designed to address physical interactions*. Generally related to buildings and equipment. (i.e., Gates, Barricades, Locks, etc.)
### Control Classifications:
> A control can (and often does) *have multiple classifications* depending upon context
- **Deterrent** - Discourages a threat agent from acting.
- **Preventative** - Stops a threat agent from being successful.
- **Detective** - Identifies and reports a threat agent.
- **Corrective**
- **Directive** - Used to increase the effectiveness of other controls. *(e.g., training)*
___
# 2.1 Security and Privacy Principles
### Information Security CIA Triad
![[ciatriad.png]]
> The three components of information security.
1. **Confidentiality**
	- The assurance that information is not disclosed to unauthorized persons, processes, or devices. 
2. **Integrity**
	- The principal that systems are trustworthy, work as intended, and the data is complete and accurate.
3. **Availability**
	- The principal that information, systems and supporting infrastructure are operating and accessible when we need.
### Supporting Principles
- **Authentication** - 
- **Authorization** - 
- **Accounting** - 
- **Non-Repudiation** - 
___
# 2.2 Zero Trust
___
# 2.3 Physical Security
___
# 2.4 Environmental Security
___
# 2.5 Deception and Disruption
___