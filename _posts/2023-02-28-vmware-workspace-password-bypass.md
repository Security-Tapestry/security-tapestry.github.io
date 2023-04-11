---
title: Security Advisory - VMWare Workspace One Password Bypass Vulnerability
categories: [Security Advisory]
tags: [security,advisory,vmware,workspace,one,password,bypass,vulnerability]
render_with_liquid: false
---
<!-- {% include emergent-banner.html %} -->
<img src="/assets/img/emergent-threat-detail-banner.png" style="margin: 0 auto; width: 100%;">

> The following is from a VMWare Security Advisory

### Impacted Products
* VMware Workspace ONE Content

### Introduction
A passcode bypass vulnerability affecting VMware Workspace ONE Content was privately reported to VMware. Updates are available to address this vulnerability in affected VMware products.

### Passcode bypass vulnerability (CVE-2023-20857)
#### Description
VMware Workspace ONE Content contains a passcode bypass vulnerability. VMware has evaluated the severity of this issue to be in the Moderate severity range with a maximum CVSSv3 base score of 6.3.

#### Known Attack Vectors
A malicious actor, with access to a users rooted device, may be able to bypass the VMware Workspace ONE Content passcode.
Resolution

To remediate CVE-2023-20857 apply the patches listed in the 'Fixed Version' column of the 'Response Matrix' below.

#### Workarounds
None.

#### Additional Documentation
None.

#### Notes
None.

### Acknowledgements
VMware would like to thank Jasper Westerman, Jan van der Put, Yanick de Pater and Harm Blankers of REQON B.V. for reporting this issue to us.

### Response Matrix

| Product               | Version | Running On | CVE Identifier | CVSSv3 | Severity | Fixed Version | Workarounds | Additional Documentation |
|-----------------------|---------|------------|----------------|--------|----------|---------------|-------------|--------------------------|
| Workspace ONE Content | Any     | Android    | CVE-2023-20857 | 6.3    | moderate | 23.02         | None        | None                     |
| Workspace ONE Content | Any     | iOS        | CVE-2023-20857 | N/A    | N/A      | Unaffected    | N/A         | N/A                      |

### References
[VMware Workspace ONE Content for Android Release Notes](https://docs.vmware.com/en/VMware-Workspace-ONE-UEM/services/rn/vmware-workspace-one-content-for-android-release-notes/index.html)

[Mitre CVE Dictionary Links](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2023-20857)

[FIRST CVSSv3 Calculator](https://www.first.org/cvss/calculator/3.1#CVSS:3.1/AV:L/AC:H/PR:L/UI:R/S:U/C:H/I:H/A:L)

### Change Log
2023-02-28: VMSA-2023-0006
Initial security advisory.

### Contact

[E-mail](mailto:security@vmware.com)

[PGP key](https://kb.vmware.com/kb/1055) 

[VMware Security Advisories](https://www.vmware.com/security/advisories)

[VMware Security Response Policy](https://www.vmware.com/support/policies/security_response.html) 

[VMware Lifecycle Support Phases](https://www.vmware.com/support/policies/lifecycle.html) 

[VMware Security & Compliance Blog](https://blogs.vmware.com/security) 

[VMWare Twitter](https://twitter.com/VMwareSRC)


<img src="/assets/img/emergent-threat-detail-banner.png" style="margin: 0 auto; width: 100%;">