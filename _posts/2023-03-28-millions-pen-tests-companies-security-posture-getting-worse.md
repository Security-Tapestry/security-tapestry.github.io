---
title: Millions of Pen Tests Show Companies' Security Postures Are Getting Worse
categories: [Cloud]
tags: [millions,penetration,testing,security,posture,getting,worse,cloud,pentesting]
render_with_liquid: false
image: /assets/img/cyberattack.webp
---

> A lack of website protections, Sender Policy Framework (SPF) records, and DNSSEC configurations leave companies open to phishing and data exfiltration attacks.

The risk score for the average company worsened in the past year as companies fail to adapt to data exfiltration techniques and adequately protect Web applications.

Companies' effective data-exfiltration risk increased to 44 out of 100 (with 100 indicating having the riskiest posture) in 2022, from an average score of 30 in the previous year, indicating that the overall risk of data being compromised has increased. That's according to rankings by Cymulate, which crunched the data on 1 million pen tests, including 1.7 million hours of offensive cybersecurity testing within its production environments.

In its "2022 State of Cybersecurity Effectiveness" report, published on March 28, the firm noted that there are various persistent problems leading to increased risk. For one, while many companies are improving their adoption and the strictness of network and group policies, attackers are adapting to sidestep such protections, the report stated. 

And the basics continue to lag: The company found that four of the top-10 CVEs identified in customer environments were more than two years old. These include the high-severity WinVerifyTrust signature validation vulnerability (CVE-2013-2900), which can allow malicious executables to pass security checks, and a memory corruption vulnerability in Microsoft Office (CVE-2018-0798).

![Cymulate Risk Scores](/assets/img/Cymulate-Risk-Scores.webp)

There is good news, however. Data from the security assessments indicates that companies have all improved risk scores for malware detection across major platforms, and many attacks are blocked by Web gateways. 

Overall, businesses need to treat cybersecurity like any other business process, with regular checks on controls, says Mike DeNapoli, director of technical messaging for Cymulate.

"Cybersecurity needs to become a process treated like any other business process, with checks and balances and regular review," he says. "The CFO would never permit the books to remain closed except for once per year, but the systems that house all that money as data routinely only get checked out during an annual pen-test, which has to change."

All of this comes against the backdrop that companies are increasingly focused on securing their entire attack surface, improving resiliency to cyberattacks, and preventing disruption of information systems. As a result, cybersecurity services and products that reduce complexity have become more popular while large technology firms have thrown their hat into the ring, such as Microsoft's launch of Defender External Attack Surface Management in August and IBM's purchase of ASM startup Randori in June. Time will tell if these trends will move the needle on risk.

![Cymulate Bar Chart](/assets/img/cymulate-security-risk-trends.webp)

While the exposure risk due to WAFs has dropped, data-exfiltration risk has increased. Source: Cymulate
Meanwhile, Cymulate's analysis of a year of offensive cybersecurity testing also found that cloud and email continue to provide rich sandboxes for hackers.

### Attacks Increasingly Coming From Popular Clouds

Attackers have shifted some aspects of their attacks away from using popular file sharing services, such as Dropbox and Box to evade email attachment filters and other security technologies, to using more generic cloud infrastructure, such as Amazon and Azure. Businesses have a harder time blocking data from large, trusted service providers, which serve as the backbone for many large cloud services and websites, DeNapoli says.

"These metrics are applied to hundreds of attempts to remove data that should be considered 'controlled' from the organization," he says. "This increase means that organizations have less control over preventing business confidential, personally identifiable, and other controlled data from being removed from the organization in unauthorized ways."

The top most successful tactics used by simulated attackers in the Cymulate research included attacking users through their browsers in a drive-by compromise scenario, archiving and exfiltrating data, and transferring that data to a cloud account, such as AWS or Azure.

### "Email Defenses Are a Team Sport"

Nearly half of the top 10 exposures uncovered by Cymulate's pen testing involved a lack of security for basic IT infrastructure. The simulations discovered that common issues included not recognizing phishing domains, a failure to configure DNSSEC, and a lack of two technologies — Domain-based Message Authentication, Reporting, and Conformance (DMARC) and Sender Policy Framework (SPF) — that can help stop email-based attacks.

Overall, companies have been slow to deploy critical email security and integrity technologies, such as DMARC, SPF, and a third technology, Domain Keys Identified Mail (DKIM) — together which can help prevent phishing success and brand fraud. While companies which implement DMARC, DKIM, and SPF records can better protect against email-based attacks, the technology standards are only truly effective if both sides of an exchange are using them, DeNapoli says.

"We need to begin to recognize that email defenses are a team sport and implement our part of the processes so others can be safer," he notes. "The benefit is that as more and more organizations implement these processes, our organization also becomes safer."

The report also showed that different industries have different strengths and weaknesses. The education and hospitality sectors, for example, had the highest risk of data exfiltration, while protections against the most immediate threats were lowest in the technology sector. Both technology and government organizations had worse-than-average Web application firewall protection.