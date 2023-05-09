---
title: SideWinder Strikes Victims in Pakistan, Turkey in Multiphase Polymorphic Attack
categories: [Attacks/Breaches]
tags: [sidewinder,strikes,victims,pakistan,turkey,multiphase,polymorphic,attack]
render_with_liquid: false
image:
  path: /assets/img/snek.webp
  alt: The APT is exploiting a remote template injection flaw to deliver malicious documents that lure in government officials and other targets with topics of potential interest.
---

India's prolific SideWinder advanced persistent threat group (APT) is targeting Pakistani government officials and individuals in Turkey, using polymorphism techniques that allow it to bypass traditional signature-based antivirus (AV) detection to deliver a next-stage payload.

The attacks use documents with content geared toward their interests, which when opened exploit a remote template injection flaw to deliver malicious payloads, the researchers at the BlackBerry Threat Research and Intelligence team revealed in a blog post on May 8.

The first phase of the campaign — discovered in November — uses a server-side polymorphic attack against targets in Pakistan, while a later phase discovered earlier this year uses phishing tactics to deliver malicious lure documents to victims, the researchers said.  

However, instead of using malicious macros within documents to drop malware — which is often the case when documents are used as lures — the APT exploits the CVE-2017-0199 vulnerability to deliver the payloads instead, the researchers said.

SideWinder, active since 2012, was detected by Kaspersky in the first quarter of 2018 and thought to primarily target Pakistani military infrastructure. However, as recent research and the latest attack demonstrate, the target range of the group — widely believed to be associated with Indian espionage interests — appears to be far broader than that.

### How Polymorphism Tricks Defenders

Server-side polymorphism is a technique used since the 1990s by attackers to evade detection by AV tools. It does so by using malicious code that alters its appearance through encryption and obfuscation, making sure that no two samples look the same and thus can't easily be analyzed, the researchers explained.

The attack can fool defenders because it serves the victim with a new sample each time a link is clicked, Dmitry Bestuzhev, senior director of cyber-threat intelligence at BlackBerry, tells Dark Reading. In this case, each new download has a new hash, which "effectively breaks hash-based detections used by security operations centers (SOCs) and some endpoint scanners," he says.

"Since there’s a new hash each time, there is no information on a given sample on public multi scanners like VirusTotal unless each new sample is uploaded over and over for further analysis," Bestuzhev says. "So it makes life harder for the victims because of the lack of information on public sandboxes and other-like security services."

### The Latest Campaign

BlackBerry researchers examined various documents in the campaign, which were found on an attacker-controlled server used to deliver the documents to users. The first that researchers encountered was titled “GUIDELINES FOR BEACON JOURNAL – 2023 PAKISTAN NAVY WAR COLLEGE (PNWC)," while another discovered in early December pretended to be a letter of offer and acceptance "for the purchase of defense articles, defense services, or both."

In both cases, targets were instructed to reach out to remote addresses controlled by SideWinder that would download the next-stage payload, “file.rtf," a rich text document file that demonstrates the polymorphic nature of the attack and can only be downloaded by users in the Pakistani IP range, the researchers said.

"The name of the file 'file.rtf' and the file type are the same; however, the contents, file size and the file hash are different," they noted. "This is an example of server-based polymorphism, where each time the server responds with a different version of file, so bypassing the victim's antivirus scanner (presuming the antivirus uses signature-based detection)."

If the user is not in the Pakistani IP range, the server returns an 8 byte RTF file that contains a single string; however, if the user is within the Pakistani IP range, the server then returns the RTF payload, which varies between 406KB to 414KB in size, the researchers said.

### To Turkey & Beyond: An Expanding Cyber Threat

In early March, the researchers discovered a new malicious document linked to the earlier attack that was propagated via phishing emails, indicating that the scope of the attack had spread to victims in Turkey — a new target region for SideWinder, researchers said. In mid-March, the researchers discovered a newly configured server delivering the payload that was set up so that a victim in Turkey could receive a second-stage payload, they said.

While SideWinder's primary targets have always been the Southeast Asia regions such as Pakistan and Sri Lanka, with a particular focus on Pakistani government institutions. However, targeting victims in Turkey makes sense from a geopolitical perspective, the researchers observed, because of the Turkish government's support of Pakistan, which has sparked criticism from India, they said.

While polymorphic attacks overall can be difficult to defend against, detection and prevention strategies based on behavior and hashes can be effectively used against them, Bestuzhev says.

"When prevention technologies are based on code similarities and heuristics or machine learning models, even if there is a new hash, it should not break the detection of the malicious sample," he notes.

The key for organizations to mitigate these attacks, Bestuzhev adds, "is not to focus on volatile indicators of compromise but on meaningful tactics, techniques, and procedures (TTPs) and behaviors in the system or code blocks covered by machine learning technologies."