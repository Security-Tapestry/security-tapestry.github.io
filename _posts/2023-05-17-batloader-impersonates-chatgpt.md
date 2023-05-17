---
title: BatLoader Impersonates ChatGPT and Midjourney in Cyber-Attacks
categories: [News]
tags: [batloader,hacker,exploit,impersonation,chatgpt,midjourney, webapp]
render_with_liquid: false
image: /assets/img/chatgpt.png
# published: false
date: 2023-05-17 13:18
---

The threat actor known as BatLoader has been observed conducting a malicious campaign using Google Search Ads to deliver imposter web pages for ChatGPT and Midjourney.

Security researchers at eSentire's Threat Response Unit (TRU) described the campaign in an advisory published on Tuesday.

“[ChatGPT and Midjourney] are extremely popular but lack first-party standalone apps (i.e., users interface with ChatGPT via their web interface while Midjourney uses Discord),” reads the technical write-up. “This vacuum has been exploited by threat actors looking to drive AI app-seekers to imposter web pages promoting fake apps.”

eSentire also explained that, in its latest campaign impersonating ChatGPT, BatLoader uses MSIX Windows App Installer files to infect devices with Redline Stealer. 

The installation involves running an executable file and a PowerShell script, which then installs and executes Redline Stealer. The script also executes two requests to the C2 panel, recording the start time and victim’s IP address and documenting the successful payload installation.

eSentire explained the technique highlights BatLoader’s ability to misuse legitimate application packaging formats for malicious purposes. Further, the threat actor has a history of targeting users searching for AI tools, as evidenced by TRU’s discovery of newly registered BatLoader domains in February 2023. 

In May 2023, TRU encountered another instance of a similar infection tactic involving an imposter page for Midjourney. Users were prompted to download a Windows Application Package signed by “Ashana Global Ltd.”

The installation process involved running an obfuscated PowerShell script identical to the script used in a previous case, but that used a different command and control (C2) domain.

“Generative AI technologies and chatbots have exploded in popularity in 2023. Unfortunately, as system administrators seek ways to control access to these platforms, users may seek out alternative ways to gain access,” reads the advisory.

To protect against these threats, eSentire recommended raising awareness of malware masquerading as legitimate applications, ensuring endpoint protection with up-to-date antivirus signatures and Next-Gen AV or EDR solutions and considering implementing Windows Defender Application Control for managing packaged apps.