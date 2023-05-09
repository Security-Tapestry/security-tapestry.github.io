---
title: Recycled Core Routers Expose Sensitive Corporate Network Info
categories: [Vulnerabilities/Threats]
tags: [recycled,core,routers,expose,sensitive,corporate,network,info,juniper,vulnerabilities]
render_with_liquid: false
image: /assets/img/racks.webp
---

> Researchers are warning about a dangerous wave of unwiped, secondhand core-routers found containing corporate network configurations, credentials, and application and customer data.

Cameron Camp had purchased a Juniper SRX240H router last year on eBay, to use in a honeypot network he was building to study remote desktop protocol (RDP) exploits, and attacks on Microsoft Exchange and industrial control systems (ICS) devices. When the longtime security researcher at Eset booted up the secondhand Juniper router, to his surprise it displayed a hostname.

After taking a closer look at the device, Camp contacted Tony Anscombe, Eset's chief security evangelist, to alert him to what he found on the router. "This thing has a whole treasure trove of Silicon Valley A-list software company information on it," Camp recalls telling Anscombe.

"We got very, very concerned," Camp says.

Camp and Anscombe decided to test their theory that this could be the tip of the iceberg for other decommissioned routers still harboring information from their previous owners' networks. They purchased several more decommissioned core routers — four Cisco Systems ASA 5500, three Fortinet FortiGate, and 11 Juniper Networks SRX Series Services Gateway routers.

After dropping a few from the mix after one failed to power up and another two were actually mirrored routers from a former cluster, they found that nine of the remaining 16 held sensitive core networking configuration information, corporate credentials, and data on corporate applications, customers, vendors, and partners. The applications exposed on the routers were from big-name software vendors used in many enterprises: Microsoft Exchange, Lync/Skype, PeopleSoft, Salesforce, Microsoft SharePoint, Spiceworks, SQL, VMWare Horizon View, voice over IP apps, File Transfer Protocol (FTP), and Lightweight Directory Access Protocol (LDAP) applications.

These network backbone devices in essence contained digital blueprints of the previous owner organizations' networks, including Border Gateway Protocol (BGP), Routing Information Protocol (RIP), and Open Shortest Path First (OSPF) routing information. The researchers "found complete layouts of various organizations' inner workings" that, in the hands of threat actors, would provide a network topology map for attack, according to the Eset researchers' white paper on the router research, released Tuesday.

The routers contained one or more set of IPSec or VPN credentials, or hashed root passwords, and each had sufficient data for the researchers to identify the actual previous owner/operator of the device. Nearly 90% included router-to-router authentication keys and details on applications connected to the networks, some 44% had network credentials to other networks (such as a supplier or partner), 33% included third-party connections to the network, and 22% harbored customer information.

"I have the entire network topology of their core infrastructure, both internal and external, like cloud assets," for example, Camp says.

Camp says the discovery was a far cry from the malware he typically studies, and a lot less work for an attacker who happened upon one of these unwiped routers. "I don't need a zero day, I have your router," quips Camp.

Abscombe and Camp say they hope to alert enterprises on the proper disposal of critical network routers when they present their findings at the RSA Conference next week.

"They are the intersection upon everything that happens in your organization," Camp says of core routers. "Everything touches the router," including many cloud services, he adds.

Recycled and repurposed computing equipment traditionally has been a fraught area. Hard drives, mobile devices, and printers over the years have been found improperly cleansed of sensitive data. In 2019, a study conducted by Rapid7 found just two out of 85 devices had been properly wiped before they were handed off to secondhand sellers or recycling services. But decommissioned and unwiped routers pose a deeper level of security risk due to the vast amount of infrastructure information they hold.

### 'Creepy' Interface
Among the organizations whose information was exposed were a manufacturing company, a US law firm, managed services providers, an open source software firm, an events company, a telecommunications equipment supplier, a global data company, and a creative services company. Eset did not disclose the names of the organizations, but the researchers confirmed that they contacted all of them.

The Silicon Valley software vendor was quick to respond, even awarding Camp a bug bounty that he then donated to the Electronic Freedom Foundation and the Tor Project. But that was the researchers' easiest disclosure.

"Once we stepped outside of the tech [sector], it was incredibly different" and harder to disclose our findings, Anscombe notes. The other organizations didn't have processes or even people available to handle the disclosure information, he says.

Meanwhile, one of the unwiped routers contained what Camp describes as a "creepy" remote administration interface.

"I was never sure if it was on purpose, but it was creepy, very low-level access, and from one of the countries with flags that we're [the US] not happy with right now," he says. "It could be totally legit or that could be really bad. It was a little edgy to me."

### How to Securely Dispose of a Core Router

So how do you wipe a router that you want to retire? The good news is most routers are fairly easy to securely decommission, and the big three — Cisco, Fortinet, and Juniper — on their websites provide detailed guidelines for restoring devices to their factory default settings.

With Juniper routers, for example, wiping the device is simple: "Going to config setting and type 'delete,' hit 'Y' [to confirm] and now that router doesn't know who it is anymore," Camp says. The entire wiping process takes less than five minutes, including the post-deletion reboot.

And if your organization already had disposed of routers that weren't properly wiped, Eset recommends rotating cryptographic keys in case an attacker were to get their hands on your old router and attempt to gain trusted access to your network. Zero trust can help here as well, they say.

But that's still no guarantee that a malicious actor who buys your old router still couldn't use it to target your organization. "Even if somebody goes and changes the credentials of the accounts being cached in router, potentially [the attacker has] got the app lists, so [they] can tell what apps are run internally locally or in the cloud," Abscombe says.

That gives the attacker just enough intel to plan a targeted attack, according to Abscombe. "If I know they're running [a specific version of] Exchange and that version had a CVE and they had not applied the patch … I suddenly know things about their network that can make them vulnerable," he says.

If you buy a secondhand core router, and, like the researchers, find that it still contains the previous owner's information, Eset recommends disconnecting the router and moving it to a secured area and contacting your regional CISA office. They also say it's best to document your purchase process as a precaution for insurance or legal purposes.