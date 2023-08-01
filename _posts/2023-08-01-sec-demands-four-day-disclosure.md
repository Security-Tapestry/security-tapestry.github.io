---
title: SEC demands four-day disclosure limit for cybersecurity breaches
categories: [Opinion]
tags: [sec,demands,disclosure,limit,breaches,cybersecurity]
render_with_liquid: false
image: /assets/img/sec.webp
date: 2023-08-01 10:45
---

Last week, the US Securities and Exchange Commission (SEC) announced new and fairly strict rules about cybersecurity breach disclosures for any people or companies that fall under its regulatory remit.

The SEC, by the way, was founded at the height of the US Great Depression in the 1930s, with the aim of preventing the sort of unregulated speculation that led to what became known as Black Thursday, the infamous Wall Street crash of 24 October 1929.

In its own words:

> The mission of the SEC is to protect investors; maintain fair, orderly, and efficient markets; and facilitate capital formation. The SEC strives to promote a market environment that is worthy of the public’s trust.

Simply put, if you’re running a company that offers shares to the public, you need to comply with the rules and regulations of the SEC, which are supposed to give your investors some sort of protection against unsubstantiated claims that disingenuously talk up a proposal, or that sneakily misrepresent the level of risk involved.

As you can imagine, especially in an online world in which ransomware breaches can bring a company to a digital standstill overnight, and where even coughing up a multimillion-dollar blackmail payment to the attackers for a “recovery program” might not be enough to get things going again…

…cybersecurity lapses can have dramatic, long-term effects on the value of a business investment.

### Demanding money with menaces

Ransomware attacks these days frequently involve cybercriminals stealing copies of your trophy data first, notably including employee and customer details, and then scrambling your copies of those very same files, thus squeezing you into a double-play cybersecurity drama.

They’ve got your files, typically including heaps of data that you were duty bound to keep to yourself, and that you had probably promised quite openly that you could be trusted with.

But you haven’t got those files any more, in any meaningful sense.

Ironically, in a typical file-scrambling ransomware attack, you can see all your files still sitting there, often with their original filenames preserved, apparently right there within clicking distance, but no more use when you try to open them than a digital pile of shredded cabbage.

Because of this double-play scenario, ransomware isn’t quite the right word these days, given that a ransom is a sum that you pay for the safe return of someone or something you want back, whether that’s a kidnapped medieval monarch or a pile of 21st-century data files.

After all, today’s “ransomware attacks” have several different ways of unfolding, including:

* __Type A.__ Your files are locked up, and only the crooks have the decryption key. Pay the exortion fee and the crooks will (or so they say) not only send you the key, but also keep quiet about what happened, so that you don’t have to admit that your temporary business outage was due to a cyberintrusion. Refuse to pay and you’re on your own. Organisations without a practicable disaster recovery plan might never get their business back on the rails at all.
* __Type B.__ Your files are copied, and the crooks have them all. Pay the extortion fee and they’ll delete the stolen data (or so they say) to shield you from data breach lawsuits from staff and customers, to stop the regulators from digging too deeply, and to help you keep your reputation intact. Refuse to pay and you’ll be firmly in the public eye, exposed as an organisation that can’t be trusted.
* __Type C.__ Both of the above.

As you can see, attacks of Type B can be pulled off even if the criminals don’t manage, or don’t want the risk of trying, to break into your network and getting access to every file directly on your own laptops, desktops and servers.

In the recent MOVEit attacks, for example, cybercrime operators allegedly working under the banner of the notorious Clop ransomware gang got hold of huge amounts of private data from numerous high-profile organisations, but without breaching those organisations directly.

Instead, the criminals went after third-party service companies such as payroll providers that transfered and stored copies of those organisations’ trophy data using the fourth-party data management product MOVEit Transfer and its online equivalent MOVEit Cloud:

And attacks of Type A can be carried out swiftly and directly, without any file exfiltration in advance, by cybercriminals who don’t want to risk getting spotted trying to upload large amounts of data.

Some crooks take that approach because any unexpected spike in outbound network traffic is a popular indicator of compromise (IoC) that businesses are learning to look out for.

In Type A ransomware attacks, the crooks don’t actually need to generate any outbound network traffic at all – not even to keep control of the magic decryption keys for each computer.

They can asymmetrically encrypt those master keys into files left behind on each affected computer, using a public key for which only they have the corresponding private key.

What a public key has locked up can’t be unlocked by that public key; only the holder of the matching private key can do that. (Think of an unlocked padlock: anyone can click it shut, but only the person with the physical key can open it up again.)

Thus the master key data is right there in plain sight, but useless to you without the necessary private key that the attackers prepared offline in advance.

All the crooks need to do is to leave behind a message telling you how to get in touch with them to start “negotiating” to buy the private key off them.

### When is a ransomware attack a notifiable breach?

One thing that’s never been obvious is just how ransomware attacks and existing data breach regulations intersect.

If you get hit by a Type A attack, but there’s no evidence that unencrypted data was exfiltrated, and you successfully restore from backups overnight and get your business back on track again quickly…

…should you be forced to tell anyone, and if so what other sorts of and scales of malware infection or data corruption should be declared too?

If you get hit by a Type B attack, and after paying the crooks off promptly you are inclined to believe that they really did delete the data so that they can no longer disclose it…

…can you reasonably define it as not-a-breach, because the data was apparently “unbreached” by the attackers, and thus no harm was ultimately done?

Indeed, if you pay out a cyberblackmail fee for any reason at all…

…should you disclose that in all cases, even where criminal law doesn’t require you to?

Unfortunately, but understandably given that this is an initial announcement, the SEC’s press release doesn’t go into that sort of detail.

Instead, it just says that those under its remit, referred to as registrants, are:

> […required to] disclose material cybersecurity incidents they experience and to disclose on an annual basis material information regarding their cybersecurity risk management, strategy, and governance.

> The new rules will require registrants to disclose […] any cybersecurity incident they determine to be material and to describe the material aspects of the incident’s nature, scope, and timing, as well as its material impact or reasonably likely material impact on the registrant.

> [The disclosure] will generally be due four business days after a registrant determines that a cybersecurity incident is material.

> The disclosure may be delayed if the United States Attorney General determines that immediate disclosure would pose a substantial risk to national security or public safety and notifies the Commission of such determination in writing.

Should paying off Type B cyberextortionists be considered “a material impact”, for example, because you can never really be sure that the crooks won’t come back for more, or that the data they stole wasn’t stolen by someone else while they had unauthorised hold of it?

Should getting hit by Type A ransomware criminals be considered “a material impact”, and if so what should the guidelines be for the scale of the attack?

In a business with a network of 100 computers, for example, how many computers would need to be scrambled in the course of a single ransomware incident for the attack to be considered likely to have exposed the business to more than just the side-effect of some ruined files?