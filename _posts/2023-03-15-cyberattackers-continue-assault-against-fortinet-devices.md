---
title: Cyberattackers Continue Assault Against Fortinet Devices
categories: [Vulnerabilities/Threats]
tags: [cyberattackers,assault,fortinet,threats,vulnerabilities,fortios]
render_with_liquid: false
image: /assets/img/fortinet.webp
---

> Patched earlier this month, a code-execution vulnerability is the latest FortiOS weakness to be exploited by attackers, who see the devices as well-placed targets for initial access operations.

In early March, a customer called in Fortinet's incident response team when multiple FortiGate security appliances stopped working, entering an error mode after the firmware failed an integrity self test.

It was a cyberattack, which led to the discovery of the latest vulnerability in Fortinet devices, a medium severity but highly exploitable bug (CVE-2022-41328) that allows a privileged attacker to read and write files. The threat group, which Fortinet labeled as an "advanced actor," appeared to be targeting government agencies or government-related organizations, the company stated in a recent analysis of the attack.

Yet the incident also shows that attackers are giving Fortinet devices significant attention. And the attack surface is wide: So far this year, 60 vulnerabilities in Fortinet products have been assigned CVEs and published in the National Vulnerability Database, double the rate at which flaws were disclosed in Fortinet devices in the previous peak year, 2021. Plenty are critical, too: Earlier this month, Fortinet revealed that a critical buffer underwrite vulnerability in FortiOS and FortiProxy (CVE-2023-25610) could allow a remote unauthenticated attacker to run any code on a variety of appliances.

Interest is high, as well. In November, for example, one security firm warned that a cybercriminal group was selling access to compromise FortiOS devices on a Russian Dark Web forum. But whether the vulnerabilities have spurred attention, or vice versa, is moot, says David Maynor, senior director of threat intelligence at Cybrary, a security training firm.

"Attackers smell blood in the water," he says. "The number and frequency of remotely exploitable vulnerabilities over the last two years has increased at a breakneck speed. If there is a nation-state group that isn't integrating Fortinet exploits, they are slouching on the job."

Like other network security appliances, Fortinet devices inhabit the critical point between the Internet and internal networks or applications, making them a valuable target to compromise for attackers looking for a foothold into corporate networks, the research team from threat intelligence firm GreyNoise Research said in an email interview with Dark Reading.

"A large majority of Fortinet devices are edge devices, and as a result are commonly Internet facing," the team said. "This is true of all edge devices. If an attacker is going to go through the effort of an exploitation campaign the volume of edge devices make[s] for a valuable target."

The researchers also warned that Fortinet is not likely alone in the crosshairs of attackers.

"All edge devices from any vendors will have vulnerabilities sooner or later," GreyNoise Research said.

### Fortinet Attack Detailed

Fortinet described the attack on its customers' devices in some detail in its advisory. The attackers had used the vulnerability to modify the device firmware and add a new firmware file. The attackers gained access to the FortiGate devices via the FortiManager software and modified the devices' start-up script to maintain persistence.

The malicious firmware could have allowed for data exfiltration, the reading and writing of files, or given the attacker a remote shell, depending on the command the software received from the command-and-control (C2) server, Fortinet stated. More than a half dozen other files were modified as well.

The incident analysis, however, lacked several critical pieces of information, such as how the attackers gained privileged access to the FortiManager software and the date of the attack, among other details. 

When contacted, the company issued a statement in response to an interview request: "We published a PSIRT advisory (FG-IR-22-369) on March 7 that details recommended next steps regarding CVE-2022-41328," the company said. "As part of our ongoing commitment to the security of our customers, Fortinet shared additional detail and analysis in the March 9 blog post and continue to advise customers to follow the guidance provided."

Overall, by finding and disclosing the vulnerability, and publishing an analysis of their incident response, Fortinet is doing the right things, the GreyNoise Research team told Dark Reading.

"They published a detailed analysis two days later including an executive summary, as well as a massive [number] of accurate details about the nature of the vulnerability and the activity of the attacker, providing defenders [with] actionable intelligence," the team stated. "Fortinet chose to clearly, timely, and accurately communicate about this vulnerability."