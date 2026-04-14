# Case 002 — LinkedIn Dual-Recruiter Social Engineering Attempt

>**Tags:** #social-engineering #phishing #linkedin #security-analysis

## Context

While maintaining a professional presence on LinkedIn, I received messages from two recruiter accounts within a short time interval.

Both messages referenced similar IT-related topics and appeared to target my professional interests.

## Observation

The interaction showed characteristics of a staged social-engineering attempt:

- the first recruiter initiated a friendly conversation related to an IT Support position
- a legitimate job posting was shared, establishing trust
- questions were asked about my experience and interests

Shortly afterwards, a second recruiter account contacted me.

The second message contained:

- information that appeared to be derived from the first conversation
- a personalized message referencing my background
- a shortened or obfuscated external link

After I refused to open the link and suggested continuing communication through normal LinkedIn channels, the recruiter quickly removed the link from the message.

## Potential Risk

Such behaviour can indicate a multi-stage social engineering attempt.

Possible attack objectives could include:

- redirecting the target to a phishing page
- harvesting credentials
- installing malware through external downloads
- gathering additional personal information

The rapid removal of the link after hesitation suggested that the link may have been malicious or inappropriate.

## Response

No external links were opened.

No credentials or personal information were shared outside LinkedIn.

The interaction was stopped once the suspicious behaviour was identified.

## Security Insight

Targeted phishing attempts on professional platforms often rely on trust-building stages.

Attackers may first establish credibility through legitimate-looking communication before delivering malicious content.



## Threat Classification

- Social Engineering  
- Phishing (potential)  
- Multi-stage reconnaissance  
- Trust-building pretexting  



## Indicators of Suspicious Activity (IoC)

- multiple recruiter accounts contacting within a short time frame  
- cross-referenced personal information between accounts  
- unsolicited external link  
- link obfuscation (shortened or masked URL)  
- behavioural change after hesitation (link removed quickly)  



## Attack Pattern

This interaction suggests a multi-stage social engineering pattern:

1. Initial contact to establish trust  
2. Use of legitimate context (real job offer)  
3. Secondary contact reinforcing credibility  
4. Delivery of external link  
5. Attempted engagement escalation  



## Conclusion

The case demonstrates a structured social engineering attempt leveraging professional context and trust-building techniques.

The use of multiple coordinated accounts and adaptive behaviour indicates a targeted approach rather than random spam.

Early identification and refusal to engage with external content prevented potential compromise.
