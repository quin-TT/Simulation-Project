[link](https://docs.google.com/open?id=1b1X_sml44a5-87f8zZ2i-2jnnqaEFSyjdqeZNi6F3m0)

APT34 Report

Analyzing APT34 (OilRig) and Defending Against Future Attacks  





1. Executive Summary
1. APT34 (also known as OilRig) is suspected to be Iran state-sponsored cyber-espionage group. They target industries such as finance, energy, and telecommunications(Mitre Att&ck) . This report inlcudes findings from trusted cybersecurity resources to answer key questions about APT34?s operations and provides  recommendations to defend against their attacks.




1. APT34 


1. APT34 has been active since 2014 (Mandiant, SecureWorks).
1. In 2017: Targeted Middle Eastern governments and energy companies using spear-phishing and custom malware like BONDUPDATER (Symantec, Kaspersky).
1. In 2019: Compromised telecommunications firms to intercept communications (CrowdStrike, CyberScoop).
1. In 2021: Used DNS tunneling to exfiltrate data from financial institutions (Recorded Future, US-CERT)
1. APT34?s long-term operations indicate high sophistication and state backing.


1. Origin and State Sponsorship 


1. APT34 has been active since 2014 (Mandiant, SecureWorks).
1. Coordination with Iranian intelligence agencies to support geopolitical goals (Mandiant, CISA).
State backing means APT34 has significant resources and persistence







1. Who are they targeting? 


1. APT34 focuses on industries critical to national infrastructure and economic stability such as:
Telecommunications: Providers in the UAE and Kuwait.

Government: Ministries and diplomatic entities (Dark Reading, The CyberWire).

Energy: Oil and gas companies (e.g., attacks on Saudi Arabian firms).

Financial Services: Banks in the Middle East.

These sectors hold classified data and critical to national security.



1. What are their motives? 


1. Cyber-Espionage: Unauthorized attempts to access trade secrets, financial data, and government intelligence.
1. Disruption: Intentional/Unintentional damaging critical infrastructure to weaken rival nations (e.g., Saudi Arabia).
1. Geopolitical Advantage: Supporting Iran?s regional influence (Recorded Future, CISA).


APT34?s motives are strategic, not financial, making them harder to deter.



1. What are the TTPs they use


1. (Mapped to MITRE ATT&CK Framework)


| Tactic  | Technique | Example | MITRE ID |
|----------|----------|----------|----------|
| Initial Access | Spear-phishing emails with malicious links | Fake job postings | T1566.002 |
| Execution | PowerShell scripts to execute malicious code. | Use to deploy malware | T1059.001 |
| Persistence | Scheduled tasks for maintenance | ?Windows update? to avoid suspicion | T1053.005 |
| Exfiltration | DNS tunneling to bypass network security. | DNS queries | T1071.004 |


                  MITRE ATT&CK, ThreatConnect, Symantec

 Understanding these TTPs helps tailor defenses to APT34?s specific methods.





1. Security measures


1. Technical Controls
Email Security:

1. Deploy AI-powered email filters (e.g., Microsoft Defender) to block spear-phishing (Dark Reading, CISA)
1. Train employees to report suspicious emails (e.g., fake job offers)
Endpoint Protection:

1. Use EDR solutions (e.g., CrowdStrike Falcon) to detect malware like BONDUPDATER (CrowdStrike).
Network Segmentation:

1. Isolate critical systems (e.g., financial databases) to limit lateral movement (MITRE ATT&CK).
Patch Management:

1. Prioritize patching vulnerabilities in public-facing apps (e.g., VPNs) (US-CERT)..


1. Operational Improvements
Threat Intelligence:

1. Subscribe to feeds (e.g., Recorded Future) for real-time APT34 IOCs (IPs, domains, malware hashes).


Zero Trust Architecture:

1. Implement ?never trust, always verify? policies for network access (CISA).
Incident Response Plan:

1. Conduct quarterly breach simulations to test response readiness (SecureWorks).


1. Strategic Initiatives
Employee Training:

1. Use phishing simulations (e.g., GoPhish) to reduce human error (The CyberWire).
Encryption:

1. Encrypt sensitive data at rest and in transit (e.g., TLS 1.3 for communications).


1. Conclusion


APT34 poses a significant threat due to its state-backed resources and focus on critical industries. By implementing the recommended technical, operational, and strategic measures, the organization can:

- Reduce the risk of spear-phishing and malware attacks.
- Detect and respond to breaches faster.
- Protect sensitive data from exfiltration.
- Conduct a risk assessment to identify high-value assets.
- Deploy EDR and email filtering solutions immediately.
- Schedule employee cybersecurity training within 30 days.














1. Report Source/s:


Picus Security. (2024, December 13). OilRig Exposed: Unveiling the Tools and Techniques of APT34. Retrieved from https://www.picussecurity.com/resource/blog/oilrig-exposed-tools-techniques-apt34



MITRE ATT&CK. (2024, September 4). OilRig. Retrieved from https://attack.mitre.org/groups/G0049/



CrowdStrike. (2018, November 27). Meet CrowdStrike?s Adversary of the Month for November: HELIX KITTEN. Retrieved from https://www.crowdstrike.com/en-us/blog/meet-crowdstrikes-adversary-of-the-month-for-november-helix-kitten/



Trend Micro. (2024, October 11). Earth Simnavaz (aka APT34) Levies Advanced Cyberattacks Against Middle East. Retrieved from https://www.trendmicro.com/en_us/research/24/j/earth-simnavaz-cyberattacks.html



Trustwave. (2025, January 29). Inside APT34 (OilRig): Tools, Techniques, and Global Cyber Threats. Retrieved from https://www.trustwave.com/en-us/resources/blogs/trustwave-blog/inside-apt34-oilrig-tools-techniques-and-global-cyber-threats/



Dark Reading. (2024, October 17). Iran's APT34 Abuses MS Exchange to Spy on Gulf Gov'ts. Retrieved from https://www.darkreading.com/cyberattacks-data-breaches/iran-apt34-ms-exchange-spy-gulf-govts



Dark Reading. (2024, October 17). Iran-Linked APT34 Spy Campaign Targets Saudis. Retrieved from https://www.darkreading.com/cyberattacks-data-breaches/iran-linked-apt34-spy-campaign-targets-saudis







