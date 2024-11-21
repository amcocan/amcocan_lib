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

| Key Terms:    | Definition:                                                                  |
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

A control can do *one*, *two*, or all *three* of these -- but it **must** do at least one of these to be considered a control.
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
- A **cost-benefit analysis** is the process of *comparing the estimated costs and benefits* to determine whether it makes sense to proceed from a business perspective.

| Key                               | Value                                                                             |
| --------------------------------- | --------------------------------------------------------------------------------- |
| Control Cost                      | The cost it takes to build, implement, and maintain the control.                  |
| Loss Cost                         | The cost of the losses without the control.                                       |
| Justified Cost                    | The cost of the control is justified.                                             |
| Unjustified Cost                  | The cost of the control is unjustified.                                           |
| Cost Justification (ROI Analysis) | An ROI analysis is required to determine the justification of the control's cost. |
```
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
A control can (and often does) *have multiple classifications* depending upon context
- **Deterrent** - Discourages a threat agent from acting.
- **Preventative** - Stops a threat agent from being successful.
- **Detective** - Identifies and reports a threat agent.
- **Corrective**
- **Directive** - Used to increase the effectiveness of other controls. *(e.g., training)*
___
# 2.1 Security and Privacy Principles
### Information Security CIA Triad
The three components of information security.
![[ciatriad.png]]
1. **Confidentiality** - The assurance that information is not disclosed to unauthorized persons, processes, or devices. 
2. **Integrity** - The principal that systems are trustworthy, work as intended, and the data is complete and accurate.
3. **Availability** - The principal that information, systems and supporting infrastructure are operating and accessible when we need.
### Supporting Principles
- **Authentication** - The process of verifying identity.
- **Authorization** - The process of approving access.
- **Accounting** - The process of tracing actions to the source.
- **Non-Repudiation** - The process of assuring the validity and origin of data.
### CIA Triad + Privacy
To expand upon the existing CIA Triad, we should add **Privacy**.

4. **Privacy** - The right of an individual to control the use of their personal information.
### Privacy Expectations
Consumers expect their privacy to be respected and their personal information to be protected be the organizations with which they do business.
- Data privacy controls relate to actions regarding collection, usage, notification, accuracy, and sharing.
- Data security controls relate to the protection mechanisms of confidentiality, integrity, and availability.
### OECD Privacy Principals
1. **Collection Limitation** - Collection of personal data should be obtained by lawful and fair means and, where appropriate, with the knowledge or consent of the data subject.
2. **Data Quality** - Personal data should be relevant to the purposes collected and should be accurate, complete, and kept up-to-date.
3. **Purpose Specification** - The purposes for which personal data is collected should be specified not later than at the time of data collection.
4. **Use Limitation** - Personal data should not be disclosed or otherwise used for purposes other than those specified except with the consent of the data subject; or by the authority of law.
5. **Security Safeguards** - Personal data should be protected by reasonable security safeguards against risks such as loss, unauthorized access, destruction, use, modification or disclosure.
6. **Openness** - Organizations should be transparent about how they handle personal data. People should easily access information about what data is collected, why it’s used, and who manages it.
7. **Individual Participation** - Individuals have the right to know if their data is held, access it easily, get reasons for denied requests, and correct or delete errors.
8. **Accountability** - A data controller must follow and uphold the above principles.
### Strategic Alignment
Every security and privacy objective must be strategically aligned with the needs of the organization.

> [!info]+ Our Mission
> Integrate the fundamental principles of confidentiality, integrity, availability, and privacy into business processes in support of organizational objectives.

___
# 2.2 Zero Trust
### Zero Trust (ZT)
A security framework requiring all subjects, assets, and workflows to be *authenticated*, *authorized*, and *continuously validated* before being granted or keeping access to applications and data.
### A Zero Trust View of a Network
1. **No Implicit Zone Trust** - The entire enterprise private network is not considered an implicit trust zone. Assets should always act as id an attacker is present on the enterprise network.
2. **No Ownership Assumptions** - Devices on the network may not be owned or configurable by the enterprise. Not all enterprise resources are on enterprise-owned infrastructure.
3. **Insecure Connections** - Remote subjects should assume that the local (i.e., non-enterprise-owned) network is hostile. Assume that all traffic is being monitored and potentially modified.
4. **Consistent Security Policy** - Assets and workloads should retain their security posture when moving to or from enterprise-owned infrastructure.
### Core Principals of Zero Trust (NIST SP800-207)
1. **Continuous Verification** - Always verify access, all the time, for all resources.
2. **Access Limitation** - Access to individual enterprise resources is granted on a per-session basis.
3. **Limit the "Blast Radius"** - Minimize impact if internal or external resources are breached. (i.e., segmentation, least privilege)
4. **Automate** - Automate context collection and response. (i.e., credentials, workloads, endpoints, SIEMS, threat intelligence)
### Control and Data Planes
In networking, a *plane* is an abstract concept of where certain processes take place. In a zero-trust environment, there is a separation of the control and data planes.
- **Control Plane** - Is used be infrastructure components to maintain and configure assets, access control, and communication security. (In a zero-trust environment, requests for access are made through the control plane.)
- **Data Plane** - Is used for communication (moving data) between software components.
### Zero Trust Architecture (ZTA)
![[Zero Trust Logical Components.png]]
### Zero Trust Logical Components
1. **Policy Decision Points (PDP)** - Functions as a gatekeeper and is comprised of two main components. (Policy Engine & Policy Administrator)
2. **Policy Engine (PE)** - Is responsible for the ultimate decision to grant access to a resource for a given subject.
3. **Policy Administrator (PA)** - Generates any session-specific authentication and authentication token, or credential used to access an enterprise resource.
4. **Policy Enforcement Point (PEP)** - Is responsible for enabling, monitoring, and eventually terminating connections between a subject and an enterprise resource.
___
# 2.3 Physical Security
### Physical Security
The protection of people, property, and physical assets from actions and events that could cause damage, loss, or unauthorized activity.

> [!info]+ Physical Security Concept
> Physical security is based upon a layered defense model. The promise of a *layered defense model* is that if an intruder can bypass one layer of controls, the next layer of controls should provide additional deterrence or detection capabilities.

- **Obstacles (Deterrent Controls)** - Used to frustrate trivial attackers and delay serious ones.
- **Detective Controls** - Used to make it likely for attacks to be noticed.
- **Response Mechanisms** - Used to catch or impede attackers.
### CPTED
The basic premise of *Crime Prevention Through Environmental Design* (CPTED) is that the proper design and effective use of the physical environment can lead to a reduction in the incidence and fear of crime, and increase safety.

> [!NOTE]+ Understanding CPTED
> CPTED relies on psychological and sociological responses.
> - People protect territory they feel is their own, and people have certain respect for the territory of others.
> - Intruders do not want to be seen.
> - Limiting access discourages intruders and/or marks them as intruders.

### Fail-Safe / Fail-Secure
There are two modes for physical security structure controls, fail-safe and fail-secure.
- **Fail-Safe** - Implies that in an emergency or fault situation, controls will default to open (unlocked).
- **Fail-Secure** - Implies that in an emergency, controls will default to closed (locked).
### Cyber and Physical Security Convergence
There is significant overlap in physical and cybersecurity controls.

> [!NOTE]+ Cyber/Physical Convergence Example
> Using a picture ID badge to identify oneself to security guards, then using the same card to "swipe" into the building, then using the same card to log into your computer with proximity technology (e.g., NFC) that automatically locks down the computer when you walk away from your desk, and produces an audit trail of your whereabouts and activity.

### Design Considerations
Structural design can be used to deter, prevent, and detect unauthorized access.
- **Data Center**
	- Located in the center of a facility with no external windows or doors.
	- Located on the floors other than the basement, first floor, and top floor.
	- Full walls extending from floor to ceiling.
	- Non-partitioned ceiling.
- **Elevators & Stairwells**
	- Keypad code.
	- RFID card access in which call buttons don't register until an authorized card is detected.
### Site Security Controls
1. **Lighting** - Used for personnel safety and intruder deterrence. Intruders are less likely to enter well-lit areas.
2. **Signs** - Used for personnel safety and intruder deterrence. Warning signs indicate surveillance.
3. **Barriers** - Walls, gates, fences, bollards, and access control vestibules define the perimeter and can be used to control and divert flow of traffic.
4. **Guards** - Stationed at checkpoints, patrol the area, manage surveillance, and respond to breaches and/or suspicious activity.
5. **Pick Resistant Lock** - A type of lock that has an extra set of tumblers which makes it resistant to picking and "bumping".
6. **Electronic Lock** - A type of lock that uses a keypad or card system and typically automatically locks doors.
7. **Smart Lock** - A type of lock that connects to a device (e.g., Bluetooth, Wi-Fi, or Z-Wave) for access control.
8. **Biometric Lock** - A type of lock that grants access based on physiological traits.
9. **Passive Infrared Sensor** - Senses change in heat signatures.
10. **Motion Sensor** - Senses changes in movement.
11. **Photometric Sensor** - Senses change in light.
12. **Acoustical Sensor** - Senses changes in noise.
13. **Contact Sensor** - Senses penetration or break in an electrical circuit.
14. **Pressure Sensor** - Senses change in surface weight.
15. **Microwave Sensor** - Senses movement within an invisible field of energy between the transmitter (Tx) and receiver (Rx).
16. **Ultrasonic Sensor** - Senses proximity of a target by converting reflected sound waves into an electrical signal.
___
# 2.4 Environmental Security
### Environmental Impact
Environmental imbalance and vulnerabilities can impact stability, availability, and integrity.
- Computers, electronic equipment, and transmission media are sensitive to environmental factors such as heat, humidity, air flow, and power quality.
- Environmental systems are often provided by and/or managed by contractors.
	- Environmental system providers should be subject to due diligence (investigation) and included in vendor management programs.
	- Environmental controls/products should be included in vulnerability management, patch management, disaster recovery, business continuity, and assessment/audit programs.
### Environmental Baselines
1. **Temperature** - Acceptable temperature for an area containing computing devices is between 18-27 degrees ℃ (64.4-80.6 degrees ℉). Circulation must take into account temperature.
2. **Humidity** - High humidity can cause corrosion and low humidity can cause excessive static electricity. Relative humidity between 50-70% is acceptable.
3. **Power** - Continuous clean (filtered) power - consistent voltage. Use of power conditioners is advised.
4. **Fire** - Fire detection and suppression capabilities.
### Hot Aisle / Cold Aisle Data Center Circulation
![[Data Center Circulation.png]]
### Power Protection
1. **Brownout** - Prolonged period with low voltage.
2. **Sag** - Moment of low voltage.
3. **Surge** - Prolonged period of high voltage.
4. **Spike** - Moment of high voltage.
5. **Blackout** - Prolonged period without power.

> [!info]+ Power Controls
> **Power Protection Controls** - Voltage Regulators, Surge Protectors, Powerline Conditioners, and Battery Backups/UPS.
> **Power Resiliency Controls** - Battery Backups/UPS, Generators, and Supplier Diversity.

### Fire Detection and Suppression

___
# 2.5 Deception and Disruption
___