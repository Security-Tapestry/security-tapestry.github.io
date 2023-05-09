---
title: Npm Packages Vulnerable to Old-School Weapon - the 'Shift' Key
categories: [Threat Intelligence]
tags: [node,js,npm,packages,vulnerable,typosquatting,old-school,weapon,shift,key]
render_with_liquid: false
image: /assets/img/npm.webp
---

> For years, hackers could have tricked enterprises into downloading malware by simply de-capitalizing letters in uppercase-named npm packages.

Since 2017, hackers have been able to mimic legitimate packages on Node Package Manager (npm) by simply removing the capital letters in their titles.

According to newly published research from Checkmarx, npm had for years failed to account for this form of typosquatting, which could have led to enterprises inadvertently downloading malware. The registry patched the vulnerability over the weekend, but organizations should be aware of any malicious packages they may have downloaded before the change was made.

"It's always good to check the names of the packages that you're installing, to make sure that you're actually installing what you want to install," says Yehuda Gelb, security researcher at Checkmarx, the author of the report. "And it's always important to have security systems in place, just to be sure."

### beware: lowercase spelling

Typosquatting occurs when cyber miscreants use deliberate but usually subtle misspellings to copy legitimate Web domains. For example, a hacker might use a capital "I" instead of a lowercase "l" in the word "Google," or zeros in place of the two "o"s.

On Dec. 26, 2017, to address typosquatting in its registry, npm announced a change to its naming system. From that date on, packages could only be named using lowercase letters. All the thousands of existing packages with capital letters in their titles remained, though, and no mechanism was implemented to prevent new packages from copying them in all but capitalization.

Consider, for instance, a package created prior to the policy change titled "localforage-memoryStorageDriver." For years, any hacker could have uploaded their own package titled "localforage-memorystoragedriver" — the exact same spelling, and all else being equal, with the only difference being no capitalized letters. An unwitting user would be forgiven for accidentally downloading the copycat.

### Exposed npm Packages

In the course of their work, the researchers found 3,815 npm packages with capital letters in their titles.

Of those, 1,900 were at risk of lowercase typosquatting. "Not all of the packages were vulnerable," Aviad Gershon, a security researcher at Checkmarx, clarifies, "because in some cases, the lowercase package names were already taken or it was not possible to register them."

Still, some extremely popular packages were exposed. The researchers pointed to objectFitPolyfill, which gets downloaded nearly 200,000 times weekly. "In total," Gelb wrote in the report, "the download count of the packages at risk is in the tens of millions."

Now that NPM has patched the flaw, malicious actors can't typosquat. "Now if you upload a new package with all lowercase letters, it's going to say the package name is too similar to an existing package, and then NPM won't allow you to upload that package," Gelb notes.

### Typosquatting's Real Risks

Rogue npm packages can compromise computers inside an enterprise network, Gershon explains. The risks in bad packages "range from information theft to ransomware, cryptomining, and denial of service," he notes.

Even an enterprise that's careful about what it downloads still faces a supply chain problem. "Packages can also be embedded in the software a supplier is distributing to their customer, and thorough that infect many other victims down the chain."

And so, awareness of typosquatting is necessary but not sufficient.

Luckily, "there are enough security solutions out there from so many different vendors — even open source ones," Gelb says.

Gershon points to Overlay — a browser extension that allows developers to evaluate packages on quality, security, and other metrics before downloading them — as an example of one of those tools that could help. "So it's something that should be easily accessible for any company."