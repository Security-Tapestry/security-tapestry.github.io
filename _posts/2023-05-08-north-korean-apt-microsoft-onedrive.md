---
title: North Korean APT Uses Malicious Microsoft OneDrive Links to Spread New Malware
categories: [Attacks/Breaches]
tags: [north,korea,apt,malicious,microsoft,onedrive,malware,attacks,breaches]
render_with_liquid: false
image:
  path: /assets/img/kim-jong-un.webp
  alt: ReconShark, aimed at gaining initial access to targeted systems, is a component of previous malware used by the Kimsuky group.
---

North Korean cyber espionage group Kimsuky has expanded its attack arsenal with a new spear-phishing campaign that uses Microsoft OneDrive links in documents armed with malicious macros that drop novel reconnaissance malware.

Researchers at SentinelLabs observed a new campaign from the threat actor targeting staff of Korea Risk Group (KRG), an information and analysis firm specializing in matters directly and indirectly impacting the Democratic People's Republic of Korea (DPRK).

They believe the same campaign is also being used to target individuals at universities — a new victim pool for Kimsuky — as well typical targets such as government organizations, research centers, and think tanks in North America, Europe, and Asia, they revealed in a recent blog post.

The campaign shows the longstanding APT wielding new malware dubbed ReconShark that's a component of — and thus named for — a custom malware variant called BabyShark previously used in campaigns toward the end of last year, SentinelOne's Tom Hegel and Aleksandar Milenkoski wrote in the post.

ReconShark can exfiltrate information, including deployed detection mechanisms and hardware information — to gain access to targeted networks, basing their assessment on overlaps in file-naming conventions, used malware staging techniques, and code format, the researchers said.

The malware appears to be "part of a Kimsuky-orchestrated reconnaissance operation that enables subsequent precision attacks, possibly involving malware specifically tailored to evade defenses and exploit platform weaknesses," the researchers wrote in the post.

## Carefully Crafted Emails

While spear-phishing is often part of Kimsuky's modus operandi, the group is paying special attention to craft emails in the latest campaign carefully, so they don't raise suspicion, the researchers said.

"[They] are made with a level of design quality tuned for specific individuals, increasing the likelihood of opening by the target," the researchers wrote. "This includes proper formatting, grammar, and visual clues, appearing legitimate to unsuspecting users."

Notably, the targeted emails, which contain links to download malicious documents, and the malicious documents themselves, abuse the names of real individuals whose expertise is relevant to the lure subject, such as political scientists, the researchers said.

The campaign against KRG specifically used Microsoft OneDrive to host the malicious document — which contains macros that execute ReconShark — presented for download in the message.

For example, a lure email used in the campaign included a OneDrive shared file link to a password protected document file named "Research Proposal-Haowen Song.doc" that contained a malicious macro for downloading the malware, they said.

Once downloaded, the main responsibility of ReconShark is to exfiltrate information about the infected platform, such as running processes, information about the battery connected to the system, and deployed endpoint threat detection mechanisms, the researchers said. The malware is similar to previous BabyShark variants in its reliance on Windows Management Instrumentation (WMI) to query process and battery information, they added.

However, ReconShark can do more than just steal data about the targeted system, the researchers said. It also can deploy further payloads in a multi-stage manner that are implemented as scripts (VBS, HTA, and Windows Batch), macro-enabled Microsoft Office templates, or Windows DLL files, they said.

"ReconShark decides what payloads to deploy depending on what detection mechanism processes run on infected machines," the researchers wrote in the post.

## Expanding its Target Base

Kimsuky, also tracked as Thallium, has been on various researchers' radar screens since 2018, and its previous activity — which SentinelOne said dates back to 2012 — has been widely reported. In earlier attacks, the group mainly focused on conducting cyber espionage against research institutions, geo-political think tanks, and — particularly during the height of the pandemic — pharmaceutical companies.

Though Kimsuky's recent activities have raised its profile among security researchers, the group appears undaunted and continues to expand its operations. In fact, the new campaign shows Kimsuky adding universities to its range of targets, which Dror Liwer, co-founder of cybersecurity company Coro, says is "worrying" due to their general lack of cybersecurity defenses and awareness programs.

"We have seen a triple-digit increase in attacks on educational institutions in the US in the last year, which is driven by a perfect storm from an attacker's perspective: Extremely valuable data, and lacking defenses," he tells Dark Reading in an email.

Overall, organizations can thwart attacks from Kimsuky and other actors' spear-phishing campaigns in general by practicing overall good email security hygiene, such as employing scanning tools to check incoming messages for suspicious activity, so they are flagged before they even reach users.

Educating employees and anyone else using an organization's email system can also help them spot malicious messages that slip through other security defenses and thus avoid compromise, experts said.