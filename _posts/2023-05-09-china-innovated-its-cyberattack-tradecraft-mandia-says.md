---
title: China 'Innovated' Its Cyberattack Tradecraft, Mandia Says
categories: [Attacks/Breaches]
tags: [china,cyberattack,tradecraft,innovation,attack,mandiant]
render_with_liquid: false
image: /assets/img/china.webp
---

> Mandiant CEO Kevin Mandia explains why a recently revealed targeted attack by a cyber-espionage group out of China rivals the SolarWinds attack in its complexity, and weighs in on how defenders can best leverage generative AI.

When more than a dozen Fortinet FortiGate firewalls mysteriously crashed and failed to properly reboot last year at a defense industry organization, it was a stroke of luck: The firewall meltdown was the first sign that intruders had deeply infiltrated the company's network in an especially stealthy and complex attack.

The attackers — which Mandiant identified as UNC3886, a lesser-known cyber-espionage hacking team out of China — appear to have misfired somehow in their campaign, causing the firewall failure, Kevin Mandia, CEO of Mandiant at Google Cloud, told Dark Reading in an interview during the RSA Conference in San Francisco last week.

"Luckily, the firewalls crashed," he says. Otherwise, it may have been "a very long time" before the attack was detected by the victim organization, according to Mandia.

Mandiant's incident response team worked with Fortinet in the breach investigation and found that the attackers had hacked into and dropped malware on FortiGate firewalls, Fortinet's management platform FortiManager, and on its log and reporting tool FortiAnalyzer. The attackers employed an old-school directory path traversal attack, exploiting a zero-day flaw in Fortinet's FortiOS (CVE-2022-41328) that let them read and write files on the firewall disks via command-line interface instructions. 

The attackers also gained super-administrator privileges in the firewalls; bypassed firewall rules on FortiManager; and set up a virtual API endpoint on FortiManager with a custom malware framework they built for VMware ESXi hypervisors and on FortiAnalyzer to anchor deep in the network infrastructure. They also disabled the system's digital signature verification step by corrupting boot files.

![Kevin Mandia. Source: Mandiant](/assets/img/kevin-mandia.webp){: .w-50 .left}
Embedding inside the firewalls and on virtual hardware kept UNC3886 out of sight from endpoint detection and response (EDR) systems that could have exposed them had they gone after workstations. That increasingly is becoming a viable alternative for the most persistent attackers, as EDR has raised the bar. "We're pushing" attacks onto firewalls as EDR improves, Mandia explains.

He says it was a near "perfect" scheme to hide in a space where they are mostly undetectable, and it's especially difficult for incident responders to uncover them and their tracks. "They could hack an infrastructure. If you’re on offense and you’re literally sitting on firewalls and virtual hardware, there's no EDR to catch you," he says.

### Heavier Lift Than SolarWinds Attack

That attack underscored a major shift in China's tradecraft, according to Mandia. "The news on offense was China had its most innovative year," he says. "Everybody got better, but China got way better" last year in its nation-state attack operations, he adds.

What was most unusual, Mandia says, was how the Chinese hacking team had meticulously deleted logs and traces of their activity on the victim's network. Hacking groups in China traditionally don't bother erasing their tracks in an attack. 

"They never really cleaned up file logs. But when they were on the Fortinet boxes, they were cleaning up their access and Web logs, doing a set of commands and then stripping out IP addresses from logs," Mandia says.

He describes the UNC3886 campaign as the "apex attack" of 2022. "This is the kind of intrusion that if you're the guy behind it, you almost see someone walking into a room saying, 'I want access to that program at that company: Go!'" he says. "More work went into that intrusion in my opinion than [it did with] SolarWinds."

China indeed had a big year in hacking. Of the 13 zero-days that Mandiant pegged as state-sponsored, seven originated from China-based APTs, according to a recent study by Mandiant. "China has a lot of resources" for cyber espionage and attacks, Mandia notes.

### AI for the Cyber Defender's Win

Meanwhile, a hot topic of late has been the use and abuse of generative AI, thanks to the whirlwind arrival of ChatGPT.

Mandia says attackers are likely to use generative AI for more targeted phishing and social engineering attacks, but he believes the technology will be especially useful for defenders and researchers. Generative AI should accelerate vulnerability discovery in addition to code development. "I feel like AI has got to be more advantageous at least on code and vulns to the defenders, because we [the defenders] know what have" before the attackers do, he says.

Mandiant currently is developing its own AI-based discovery tool. "We are working on a malware analysis capability on that," he says. "The fact that we might be able to just take malware and pop it into the an engine and 15 seconds later get a great report on it: that's a defender's advantage."

"AI is going to be a shift change," he says. "You can feel it."