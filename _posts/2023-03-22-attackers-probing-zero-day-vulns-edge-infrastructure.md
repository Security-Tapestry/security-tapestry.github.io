---
title: Attackers Are Probing for Zero-Day Vulns in Edge Infrastructure Products
categories: [Attacks/Breaches]
tags: [attackers,probing,zero-day,vulnerabilities,edge,infrastructure,products,attacks,breaches]
render_with_liquid: false
image: /assets/img/zero-day.webp
---

> Nearly 20% of the zero-day flaws that attackers exploited in 2022 were in network, security, and IT management products, Mandiant says.

An analysis of data associated with zero-day attacks in 2022 suggests that threat actors are increasingly probing for security weaknesses in edge-infrastructure technologies, including VPNs, firewalls, and IT management products.

Researchers from Mandiant tracked a total of 55 zero-day vulnerabilities that adversaries exploited in various malicious campaigns last year and found that 10 of them involved an Internet-facing edge device.

Among them were CVE-2022-1040 and CVE-2022-3236 in Sophos firewalls, CVE-2022-20821 in Cisco IOS, CVE-2022-42474 and CVE-2022-41226 in Fortinet's FortiOS, CVE-2022-288810 in Zoho ManageEngine, and CVE-2022-35247 in SolarWinds Serv-u.

### Hunting on the Edge

Casey Charrier, Mandiant senior analyst at Google Cloud, says adversaries are focusing on edge technologies likely because they perceive enterprise organizations as having fewer capabilities around endpoint detection and response (EDR) than they have around network monitoring.

"That's definitely an element that we assess is a focus of Chinese threat groups right now," Charrier says. "As more organizations integrate Internet of Things (IoT) devices into their environment, they'll need to take this into consideration when evaluating security tools and the security of these devices."

The 55 zero-days that Mandiant observed adversaries using in 2022 are fewer than the all-time high of 81 that its researchers observed in 2021. Even so, the number was nearly three times higher than the 20 zero-days Mandiant observed being exploited in 2020.

### Chinese Actors Continue to Be Most Active Exploiters of Zero-Days

As has been the case for some time now, Chinese state-sponsored threat groups exploited more zero-days in 2022 than any other threat group. Of the 13 zero-days that Mandiant was able to identify as likely exploited by a state-backed group, seven — or more than half — involved a Chinese advanced persistent threat (APT) group.

One example is CVE-2022-30190, a vulnerability in the Microsoft Windows Support Diagnostic Tool that enables remote code execution (RCE) via malicious Office documents, even when a user might have disabled macros. Chinese threat actors used the vulnerability, also referred to as "Follina," in numerous threat campaigns throughout the year, making it one of the most heavily exploited flaws of 2022.

Several of the zero-days that Chinese state actors leveraged in attacks last year targeted network devices. One example is CVE-2022-42475, a buffer-overflow flaw in FortiOS SSL VPN technology that a China-based actor used in a campaign last year to deliver a highly customized tool for exploiting Fortinet's FortiGate firewalls. Another flaw in this category that a Chinese actor abused is CVE-2022-41328, a path traversal vulnerability in FortiOS. Mandiant observed a Chinese group identified as UNC3886 exploiting the vulnerability in a potential cyber-espionage campaign. The same actor was previously associated with an attack campaign targeting VMware ESXi hypervisors using a new technique with malicious vSphere Installation Bundles.

Mandiant said it also observed zero-day exploit activity involving North Korean threat actors ticking up slightly in 2022 compared with previous years. The two zero-days that Mandiant identified North Korean actors exploiting were: CVE-2022-0609, a Google Chrome vulnerability that a North Korean group exploited in a campaign targeting the high tech, media, and financial sectors, and CVE-2022-41128, an RCE in Windows Server that North Korea's APT37 exploited in a phishing campaign.

### Financially Motivated Cyberattackers Want in on the Action Too

Financially motivated threat actors continued to be another set of adversaries that actively exploited zero-day vulnerabilities last year, though not to the same extent as in 2021. Of the 16 zero-days for which Mandiant was able to attribute a motive, four were used in financially motivated attacks. Many of these attacks involved ransomware deployments. Examples include CVE-2022-29499, an RCE flaw in a Mitel VoIP appliance that a threat actor used to deploy Lorenz ransomware, and CVE-2022-41091, i.e. a Windows Mark of the Web flaw that the operator of the Magniber ransomware used in one campaign.

Since 2019, zero-day exploit activity involving ransomware groups has been increasing, says Charrier. "This is the case for a variety of reasons," Charrier notes. "For one, ransomware, as a proportion of all financially motivated activity, has continued to grow and take over the criminal ecosystem. Second, it can be more obfuscated in terms of tracking the money as well as tracking any sort of victim payments."

Microsoft, Google, and Apple topped the charts — as they always have — in terms of the number of zero-day vulnerabilities in their respective products. The three vendors together accounted for 37 of the 55 zero-days that Mandiant tracked last year. Fifteen of the zero-days in operating systems affected Windows and nine out of 11 browser zero-days were in Google Chrome.

At the same time, the number of zero-days that threat actors found and exploited in other technologies grew as well. As zero-day numbers increase, so do the number of vendors that are victims, Charrier says: "While the top three targeted vendors remain consistent, the variety of additional targeted vendors generally continues to expand and vary each year."