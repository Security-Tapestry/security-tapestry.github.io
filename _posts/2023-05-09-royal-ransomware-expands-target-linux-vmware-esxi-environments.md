---
title: Royal Ransomware Expands to Target Linux, VMware ESXi
categories: [Threat Intelligence]
tags: [royal,ransomware,threat,intelligence,linux,vmware,esxi,batloader,attacks]
render_with_liquid: false
image: /assets/img/royal.webp
---

> The ransomware gang has also started using the BatLoader dropper and SEO poisoning for initial access.

The Royal ransomware group — which is made up of former members of the Conti gang — has ramped up operations since bursting on the scene last summer, mounting attacks against critical infrastructure and healthcare targets in particular. Most recently, it has expanded its arsenal to target Linux and VMware ESXi environments.

That's according to Palo Alto Networks' Unit 42 division, who noted in an analysis released May 9 that the group has recently launched a variant of its encryptor malware built in the form of executable and linkable format (ELF) binary.

"[It] is quite similar to the Windows variant, and the sample does not contain any obfuscation," the researchers explained in the posting. "All strings, including the RSA public key and ransom note, are stored as plaintext."

Linux runs the back-end systems of many networks and container-based solutions for Internet of Things devices and mission-critical applications, and as such, represents a plum attack surface for threat actors interested in disrupting critical operations.

VMware's ESXi platform meanwhile is an increasingly attractive target for ransomware attackers, with multiple ransomware campaigns targeting the virtualization platform in the past year alone. There's the added benefit of bang for the buck: A compromise of one ESXi hypervisor could open the door to all of the virtual machines (VMs) that it controls, without any additional work.

"Considering many ransomware families have an ESXi/Linux focused variant, this isn't unusual," Unit 42 researchers said. "It only makes sense that this group would expand their arsenal to impact other environments."

### Royal Ransomware: Heir to the Crown of Conti

Other researchers previously determined that Royal is likely is made up mainly of former members of the Conti ransomware group — specifically, ex-members known as "Team One," according to Unit 42.

Conti, which was responsible for the Ryuk ransomware, famously disbanded last May when the gang's developers began shutting down admin panels, servers, proxy hosts, chatrooms, and a negotiations service site — likely in response to law enforcement and media attention. At the time, researchers noted that it would be likely that members would regroup under new guises — and that's exactly what appears to have occurred.

"Because some of the people behind this threat were part of the development of Ryuk, which is the predecessor of Conti, they have many years of experience," according to Unit 42 researchers. "This means they have a solid base for carrying out attacks and know what works when extorting victims."

Unit 42 incident responders have participated in 15 cases involving Royal ransomware in the last nine months (with demands of up to $25 million in Bitcoin). But Royal's romp has been broader and more extensive than even that, with Unit 42 totting up hits on 14 manufacturing organizations in 2022, and 26 more in 2023. It has also impacted 14 organizations in the education sector, according to the analysis, and eight healthcare organizations since the gang started, prompting the US Department of Health and Human Services to issue a warning about the group in January.

Most recently, the group claimed responsibility for an attack on the City of Dallas last week that left government systems out of service, including the Dallas Police Department website.

Most of the organizations impacted by Royal are in the US and Canada, making up 73% of the attacks, according to Unit 42.

### Royal Takes Off With BatLoader

Another recent change to the cybercrime gang's tactics, techniques and procedures (TTPs) is the use of the BatLoader first-stage malware dropper, Unit 42 researchers said.

"The Unit 42 team has observed this group compromising victims through a BatLoader infection, which threat actors usually spread through search engine optimization (SEO) poisoning," according to the posting. "This infection involves dropping a Cobalt Strike beacon as a precursor to the ransomware execution."

Royal is notable for bucking the trend towards using a ransomware-as-a-service (RaaS) model as Conti did — i.e., rather than partnering with affiliates to carry out the attacks in exchange for a profit share, Royal operates as a private group, doing its own dirty work.

That said, the use of BatLoader might indicate that Royal might be forging partnerships to achieve initial access at targeted organizations.

The same infection routine using BatLoader and SEO poisoning (aka malvertising) was previously seen in November — but in that case, the dropper was seen being used to ultimately deliver a range of end-stage malware, not just ransomware, suggesting that its operators offer the tool to a variety of threat actors.

### How to Defend Against a Royal Pain

"Royal ransomware has been more active this year, using a wide variety of tools and more aggressively targeting critical infrastructure organizations," according to the Unit 42 posting. "Organizations should implement security best practices and be wary of the ongoing threat of ransomware."

To defend themselves, the Unit 42 team recommends that organizations implement advanced logging capabilities, including tools such as Sysmon, Windows command-line logging, and PowerShell logging.

"Ideally, you should be forwarding these logs to a security information and event management tool (SIEM) to create queries and detection opportunities," researchers recommended. "Keep computer systems patched and up to date wherever possible to reduce the attack surface related to exploitation techniques. Deploy an extended/endpoint detection & response (XDR/EDR) solution to perform in-memory inspection and detect process injection techniques."