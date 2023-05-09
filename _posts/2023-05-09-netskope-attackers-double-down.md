---
title: Netskope - Attackers Double Down on Social Engineering Techniques and Malicious Functionalities
categories: [Attacks/Breaches]
tags: [netskope,attackers,social,engineering,techniques,malicious,functionalities]
render_with_liquid: false
# image:
#   path: /assets/img/nextgen.webp
#   alt: alt text
---

> Researchers find attackers are successfully evading detection by blending in with normal network traffic via HTTP and HTTPS.

**SANTA CLARA, Calif. – May 2, 2023** – Netskope, a leader in Secure Access Service Edge (SASE), today unveiled new research confirming that attackers are finding new ways to evade detection and blend in with normal network traffic using HTTP and HTTPS to deliver malware. In its latest Cloud & Threat Report: Global Cloud and Web Malware Trends, Netskope identified that on average, five out of every 1,000 enterprise users attempted to download malware in Q1 2023, and new malware families and variants represented 72% of those malware downloads. 

### Social Engineering and Search Engine Data Voids on the Rise

In the research, Netskope uncovered that nearly 10% of all malware downloads in Q1 were referred from search engines. These downloads mostly resulted from weaponized data voids, or combinations of search terms that have very few results, which means that any content matching those terms is likely to appear very high in the search results. This represents just one of many social engineering techniques that attackers are accelerating.

Social engineering as a whole continues to dominate as a leading malware infiltration technique with attackers abusing not only search engines, but email, collaboration apps, and chat apps to trick their victims. As the top two malware types, Trojans accounted for 60% of malware downloads in Q1 and phishing downloads accounted for 13%.

### Evaluation of Primary Communication Channels for Attackers 

For the first time in its quarterly cloud and threat reporting, Netskope analyzed attacker communication channels. Researchers found that attackers, in order to consistently evade detection, have used HTTP and HTTPS over ports 80 and 443 as their primary communication channel. In fact, of the new malware executables analyzed by Netskope that communicated with external hosts, 85% did so over port 80 (HTTP) and 67% did so over port 443 (HTTPS). This approach enables attackers to easily go unnoticed and blend in with the abundance of HTTP and HTTPS traffic already on the network. 

Additionally, to evade DNS-based security controls, some malware samples sidestep DNS lookups, instead reaching out directly to remote hosts using their IP addresses. In Q1 2023, most malware samples that initiated external communications did so using a combination of IP addresses and hostnames, with 61% communicating directly with at least one IP address and 91% communicating with at least one host via a DNS lookup.

"Job number one for attackers is finding new ways to cover their tracks as enterprises put more resources into threat detection, but these findings indicate just how easy it still is for attackers to do so in plain sight," said Ray Canzanese, Threat Research Director, Netskope Threat Labs. “As attackers gravitate towards cloud services that are widely used in the enterprise and leverage popular channels to communicate, cross-functional risk mitigation is more necessary than ever.” 

### Extended Look into Global Cloud and Web Malware Trends

Other notable findings uncovered by Netskope’s research team include:

* **55% of HTTP/HTTPS malware downloads came from cloud apps**, up from 35% for the same period one year earlier. The primary driver of the increase is an increase in malware downloads from the most popular enterprise cloud applications, with **Microsoft OneDrive tracked as the most popular enterprise app by a wide margin**.
* The number of applications with malware downloads also continued to increase, **reaching a high of 261 distinct apps in Q1 2023**.
* **Only a small fraction of total web malware downloads were delivered over web categories traditionally considered risky**. Instead, downloads are spread out among a wide variety of sites, with content servers (CDNs) responsible for the largest slice, at 7.7%.

As enterprises work to defend against the onslaught of malware, cross-functional collaboration across multiple teams is required, including network, security operations, incident response, leadership, and even individual contributors. Some of the additional steps organizations can take to reduce risks include: 

* Inspect all HTTP and HTTPS downloads, including all web and cloud traffic, to prevent malware from infiltrating your network
* Ensure that security controls recursively inspect the content of popular archive files and that high-risk file types are thoroughly inspected
* Configure policies to block downloads from apps that are not used in your organization to reduce risk surface.

For more information on cloud-enabled threats and our latest findings from Netskope Threat Labs, visit Netskope's Threat Research Hub.

### About Netskope

Netskope, a global SASE leader, is redefining cloud, data, and network security to help organizations apply zero trust principles to protect data. Fast and easy to use, the Netskope platform provides optimized access and real-time security for people, devices, and data anywhere they go. Netskope helps customers reduce risk, accelerate performance, and get unrivaled visibility into any cloud, web, and private application activity. Thousands of customers, including more than 25 of the Fortune 100, trust Netskope and its powerful NewEdge network to address evolving threats, new risks, technology shifts, organizational and network changes, and new regulatory requirements. Learn how Netskope helps customers be ready for anything on their SASE journey, visit netskope.com.