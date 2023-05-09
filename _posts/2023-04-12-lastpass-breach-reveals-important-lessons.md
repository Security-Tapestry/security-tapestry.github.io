---
title: LastPass Breach Reveals Important Lessons
categories: [Attacks/Breaches]
tags: [lastpass,breach,passwords,important,lessons,attacks,cyberattacks]
render_with_liquid: false
image: /assets/img/lastpass.webp
---

> Devastating cyberattacks often can be prevented with basic cybersecurity measures.

The LastPass breach will be remembered as paradigmatic. The blast radius from this August 2022 breach grew from bad to catastrophic during a six-month period. Initially, the LastPass CEO declared the breach contained. However, in November 2022, an unknown threat actor was discovered to have accessed the LastPass' cloud-based storage environment and encrypted password vaults using information obtained during the August incident. By the end of the year, LastPass confirmed that customer data, including encrypted passwords and usernames, had been compromised. 

On March 3, it was revealed that the root cause of the LastPass data breach was surprisingly basic. The attacker compromised a LastPass DevOps engineer's personal computer through an old vulnerability in a third-party media software package called Plex, which was apparently used by an employee for personal purposes. Consequently, the computer was infected with a keylogger, allowing threat actors to steal partially encrypted password vault data and customer information. 

The recently revealed details of the LastPass data breach provide important lessons for organizations, particularly security companies. 

### Adhere to Your BYOD Policy: A Must for Privileged Users

It's concerning that four LastPass engineers with access to highly sensitive assets were able to use their personal devices, including personal applications, for work purposes. Personal devices often lack the same security protocols and patches as company-issued devices, and they may be used by family members or for non-work-related activities, which can significantly increase the risk of compromise. According to a survey by Action1, 43% of IT professionals reported that the top risky behavior remote workers are susceptible to is allowing family members to use corporate devices for activities unrelated to work.

To mitigate these risks, organizations should have strict security policies that apply to all users, particularly privileged ones. Issuing company-owned devices subject to regular security updates and protocols is the best practice. However, in situations where personal devices are used for work, it's essential to establish a robust bring-your-own-device (BYOD) policy, ensuring that personal machines follow the same security measures as company-issued devices, including regular updates, anti-malware software, and multifactor authentication (MFA). 

### Don't Let Legacy Vulnerabilities Put Your Endpoints at Risk

In the LastPass breach, the attacker exploited a vulnerability in a third-party media software package called Plex. Although Plex had issued a patch for the vulnerability 75 versions ago, the employee's machine at LastPass had not been updated. This underscores the importance of companies remaining vigilant in their patch management, especially for third-party software. It's also essential to monitor the software installed on employees' machines and ensure that it adheres to corporate security policies. However, it's not just legacy security vulnerabilities that can be found in unapproved third-party software — they can also exist in commonly used apps like browsers. It’s hard to underestimate the importance of automated patch management for both OS and third-party applications in cybersecurity.

### Avoid Easily Bypassed MFA

The LastPass breach highlights the limitations of MFA. In that incident, keylogging malware captured an employee's MFA token, allowing the attacker to bypass this security measure. This shows that not all MFA methods are equally secure. 

The thing is, despite the popularity of MFA, some organizations may have adopted it without fully understanding the nuances of different MFA methods. There are many services that provide authentication via SMS, email, or authentication applications. However, the reality is that MFA with hardware tokens is the most secure one. Hardware tokens generate unique passcodes that are difficult to intercept or replicate, and they do not rely on Internet or cellular connections and should be considered for securing access to services with highly sensitive assets. 

### Build Security Into Your Products and Infrastructure From the Start

Although LastPass declared advanced security measures for their products, the breach revealed gaps in various areas. For example, LastPass stored MFA seeds and the split knowledge component (K2) key together, which allowed threat actors to access them after obtaining decryption keys for encrypted backups of the LastPass MFA/federation database. It would have been more prudent to store these highly sensitive assets separately. Additionally, although LastPass requires users to implement strong master passwords, these measures are not always enforced, and notifications may not be noticeable enough, as indicated by some experts. 

This suggests that a typical situation occurred where IT architecture develops in response to business demand for meeting the needs and capturing the market, and IT security is incorporated into the architecture only later on. As a result, it becomes difficult to incorporate security policies and redesign the architecture accordingly. Therefore, it's better to consider IT security from the outset of product development. 

### Conclusion

Devastating cyberattacks often can be prevented with basic cybersecurity measures, yet even security companies can make mistakes. We should learn from these errors to improve our own security practices. 