---
title: Emotet, QSnatch Malware Dominate Malicious DNS Traffic
categories: [Threat Intelligence]
tags: [emotet,qsnatch,malware,dominate,malicious,dns,traffic,intelligence,threat,enterprise]
render_with_liquid: false
image: /assets/img/dns.webp
---

> An analysis of trillions of DNS requests shows a shocking amount of malicious traffic inside enterprise networks, with threats using DNS as a sort of malicious Autobahn.

The Internet's domain name system (DNS) has become a superhighway of sorts for threat actors, with one in six organizations experiencing malicious network traffic in the form of either malware such as Emotet, phishing attacks, or command-and-control (C2) activity in an given quarter, researchers have found.

Researchers from Akamai looked at data from more than than 7 trillion daily DNS requests to examine how threat actors are leveraging the servers and devices enterprises use to manage these requests to conduct their nefarious activity.

What they found is that attackers are zooming in and out of networks via DNS at an alarming frequency, with between 23% and 27% of organizations experiencing at least one instance in which C2 traffic was observed traveling out of their network in any given quarter, the Akamai researchers said in a report published today.

This traffic provides "a very accurate predictor for attacks in progress, and can provide a very accurate image of the threat landscape," says Eliad Kimhy, cybersecurity research team lead at Akamai.

Moreover, much of this traffic is occurring in real time, making it harder for the enterprise to defend against it, he adds.

"Attackers are increasingly operating with a 'hands on keyboard' philosophy, giving the job of hacking an organization to a live operator," Kimhy says. "This is going to make detecting and stopping C2 traffic a crucial aspect of an organization's security, and we will likely see this play an ever-growing role in the modern attack."

### Emotet, QSnatch & the Current State of Attacks

The Akamai researchers reported a range of findings about not only how attackers are using DNS, but what type of attacks and malware are most prevalent in their observations. One of the most interesting was that the stalwart threat Emotet, which resurfaced recently after a brief hiatus, is not only back, but back with a vengeance.

"It is prevalent and seems to conduct massive campaigns to try and breach organizations," Kimhy says.

The researchers observed one "massive campaign" last year, and it appears that the threat group is ramping up for another, he says. "This is a very difficult group to contend with, as it specializes in breaching and selling access to more dangerous groups, like ransomware groups," Kimhy notes.

Moreover, this resurgence of Emotet is a good indicator that more attacks — potentially from ransomware groups — are on the horizon, as the malware is often used as an initial access to networks, he says.

In fact, the researchers found that 9% of infected network devices that they observed reaching out to C2s accessed domains associated with ransomware-as-a-service (RaaS) group, demonstrating the continued risk from ransomware attacks with business-crippling consequences — including remediation and recovery costs, legal fees, fines, downtime resulting in loss of productivity, and brand and reputation damages — for the enterprise.

Attackers also are increasingly finding their way into organizations' networks via network-attached storage (NAS) devices on the back of the botnet QSnatch, with more than a third of affected devices that researchers observed showing traffic leading to C2 domains related to this threat, the researchers found.

These devices can represent "a huge threat surface" if they're not well-secured, as organizations often use NAS devices for backups and the storage of crucial data, according to Akamai.

"Finding yourself in a position where your data is stolen or backups are deleted in support of a ransomware attack can be a terrible position to be in," Kimhy says.

In terms of which types of organizations attackers go after using DNS, the researchers found that manufacturing, business services, and retail are facing the highest risk, though no industry is safe from imminent attack.

### How Cyber Defenders Can Protect Against DNS Threats

Given the insight about the current malicious activity hitching a ride into enterprise networks via DNS, security administrators can now arm themselves against the most prevalent threats targeting their networks. One way to do this is to conduct gap assessments and close those gaps where necessary, the researchers said.

Overall, given the current threat landscape, knowledge is power, Kimhy says. "Security teams need to know who’s on the other side of the attack — and which groups put their organization at risk — in order for them to be able to defend," he says.

Moreover, the "broken record" advice of adopting a "zero trust" mentality continues to ring true, with the deployment of "products that specialize in stopping an attack that has gone past the perimeter" — such as endpoint detection and response (EDR), microsegmentation, and secure Web gateways (SWGs) — offering particular advantage in defending against the current threat landscape, the researchers said.

Given the advanced threat posed to NAS devices, the Akamai researchers also recommended that organizations ensure any that companies have on their network be securely nailed down. "It is strongly advised that security teams ensure their NAS devices are up to date," Kimhy says "and properly secured via segmentation, or other appropriate tools."