---
title: Attacker uses the Azure Serial Console to gain access to Microsoft VM
categories: [News]
tags: [attacks,azure,serial,console,microsoft,vm,rmeote,management,virtual,machines]
render_with_liquid: false
image: /assets/img/theft-fraud.webp
# published: false
date: 2023-05-17 10:21
---

> Using the access to virtual machines the attackers employed malicious use of the Serial Console on Azure Virtual Machines to install third-party remote management software within client environments.

Financially motivated threat actor UNC3944 is using phishing and SIM swapping attacks to take over Microsoft Azure admin accounts and gain access to virtual machines (VM), according to cybersecurity firm Mandiant.

Using access to virtual machines the attackers employed malicious use of the Serial Console on Azure Virtual Machines to install third-party remote management software within client environments, Mandiant said in a blog.

UNC3944 has been active since May 2022. The threat actor has been observed carrying out SIM-swapping attacks followed by the establishment of persistence using compromised accounts.

Once persistence has been established, UNC3944 has been seen modifying and stealing data from within the victim organization’s environment. “This threat group heavily relies on email and SMS phishing attacks and has also been observed attempting to phish other users within an organization once they’ve gained access to employee databases,” Mandiant said.

### Smishing used by threat actors

The threat actor leverages compromised credentials of administrators or other privileged accounts for initial access. A common tactic employed by this attacker involves smishing of privileged users, SIM swapping, and then impersonating the users to trick helpdesk agents into sending a multi-factor reset code via SMS, Mandiant said.

Once the threat actor has gained access to the Azure administrator’s account, they gain full access to the Azure tenant as administrator accounts have global privileges granted. With full access to the tenant, the threat actor can export information about the users in the tenant, gather information about the Azure environment configuration and the various VMs, and create or modify accounts.

Mandiant researchers have observed the threat actor using their access to a highly privileged Azure account to leverage Azure Extensions for reconnaissance purposes.

### Using extensions for information gathering 

After gaining access to the Azure environment, the threat actor uses the built-in Azure diagnostic extensions for information-gathering purposes, Mandiant said. 

Azure Extensions are additional features and services that can be integrated into an Azure Virtual Machine to expand capabilities and automate tasks. The extension CollectGuestLogs which can be used to gather log files for offline analysis and preservation is one such extension leveraged by the threat actor.

“Once the attacker completes their reconnaissance, they employ the Serial Console functionality to gain an administrative command prompt inside of an Azure VM,” Mandiant said. The threat actor then runs a command which identifies the name of the currently logged-in user.

“To maintain a presence on the VM, the attacker often deploys multiple commercially available remote administration tools via PowerShell,” Mandiant said, adding that the advantage of using these tools is that they’re legitimately signed applications and provide the attacker remote access without triggering alerts in many endpoint detection platforms. 

UNC3944 also creates a reverse SSH tunnel to their command and control server, to maintain access via a secure channel and bypass network restrictions and security controls. The reverse tunnel is configured with port forwarding, facilitating a direct connection to Azure Virtual Machine via Remote Desktop.

“Following the creation of the SSH tunnel, the attacker established a connection to the SSH tunnel using their current account or by compromising additional user accounts and leveraging them to connect to the compromised system via Remote Desktop,” Mandiant said.

### Living off the land attacks
Living off the land attacks like these have become far more common as attackers have learned to make use of built-in tools to evade detection, Mandiant said. “The novel use of the Serial Console by attackers is a reminder that these attacks are no longer limited to the operating system layer.” 

Land attacks are the ones where attackers use legitimate tools within the victim’s systems to carry out their attacks.

Mandiant is recommending that organizations restrict access to remote administration channels and disable SMS as a multifactor authentication method wherever possible. It is also recommended to review user account permissions for overly permissive users and implement appropriate Conditional Access Authentication Strength policies.