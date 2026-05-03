Case 005 — Multi-Channel Social Engineering via Banking Workflow (Anonymized)

Tags: #phishing #vishing #social-engineering #email-security #sms #mitre

A real-world multi-channel social engineering attempt leveraging legitimate banking infrastructure.
The name of the bank is intentionally anonymized.
Context
The user received multiple messages related to account activation.
The communication included:

• email messages from a legitimate banking domain

• SMS messages with similar content

• instructions to contact a support number

The messages appeared urgent and security-related.

Observation
• email passed SPF, DKIM, and DMARC checks

• no suspicious links were present

• phone number was included inside the message body

• SMS and email content were consistent

• multiple messages were received in a short time

The communication pattern differed from standard banking notifications.
Attack Flow (Simplified)

1.Attacker obtains victim’s email and phone number

2.Attacker triggers legitimate banking process

3.Bank system sends authenticated email

4.Email includes attacker-controlled phone number

5.Attacker sends matching SMS

6.Victim is encouraged to call support

7.Attack continues via phone (vishing)

Key Weakness Exploited
The attack does not break authentication.

Instead, it abuses:
•trusted communication channel

•legitimate infrastructure

•insufficient validation of dynamic content

•user trust

Why This Attack Is Effective

•email is technically legitimate (SPF/DKIM pass)

•no malicious links

•multi-channel consistency (email + SMS)

•urgency and fear trigger

Result:
→ victim initiates contact voluntarily
Attack Flow Diagram
flowchart TD
    A[Attacker obtains data] --> B[Trigger banking process]
    B --> C[Bank sends real email]
    C --> D[Injected phone number]
    B --> E[SMS sent]
    D --> F[Victim receives email]
    E --> F
    F --> G[Victim calls]
    G --> H[Vishing attack]


## MITRE ATT&CK Mapping

| Tactic              | Technique     | Description               |
|--------------------|--------------|---------------------------|
| Reconnaissance     | T1589        | Victim data collection    |
| Initial Access     | T1566        | Phishing                  |
| Execution          | T1204        | User interaction          |
| Credential Access  | T1056        | Data extraction           |
| Impact             | T1566.004    | Vishing                   |

Attack Hypothesis vs Evidence
Hypothesis 1: Email spoofing
 Not supported (SPF/DKIM pass)
 
Hypothesis 2: System compromise
 No evidence
 
Hypothesis 3: Workflow abuse
 Likely
 
Hypothesis 4: Multi-channel attack
 Strongly supported

Response

no interaction with attacker
no data shared
case reported to bank

Bank Response

The bank confirmed:
the communication is fraudulent
users are not asked to act via such messages
case forwarded to security team

Conclusion

This incident represents a multi-channel social engineering attack using legitimate infrastructure.
No system compromise was required.
The attack relied on:
→ user trust
→ coordinated communication
→ behavioral manipulation

Key Insight

Technical validation alone is not sufficient.
→ Behavioral analysis is critical in detecting modern phishing attacks.
