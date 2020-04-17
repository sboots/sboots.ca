---
title: "Corporate networks are not the future"
date: 2020-04-15T22:40:08-07:00
summary: "It’s been about a month now since federal government employees have been asked to work from home. The sudden shift to a fully remote workforce quickly overwhelmed the IT infrastructure used to access corporate networks from home. The future fix to this problem is to move away from having corporate networks entirely."
subtitle: "The future is speed and reliability, brought to you by regular internet connections"
images: ["/img/2020/bellmar-strangeloop-tic-presentation.jpg"]
---

It’s been about a month now since federal government employees have been [asked to work from home](https://www.canada.ca/en/government/publicservice/covid-19.html), to reduce the potential spread of the COVID-19 pandemic. This has been a fairly unprecedented change for the public service. 

Across hundreds of thousands of public service employees, only a small fraction normally work from home – and the sudden shift to a fully remote workforce quickly overwhelmed the IT infrastructure used to access corporate networks from home. As [this piece from Chris Nardi explains](https://nationalpost.com/news/canada/thousands-of-federal-employees-to-receive-paid-vacation-since-they-cant-work-from-home),

> Since Monday, most federal departments are asking staff who were sent home to stay off internal servers if they aren’t working on core or critical services. That’s because most ministries have significant limitations on how many people can simultaneously access work servers from outside the office.

> “Imagine when you used to have to connect to the Internet with a dial-up connection. That’s what the situation is now. Every minute counts, so you connect, you download what you need, and then you get off,” union leader Debi Daviau said about government VPNs (Virtual Privacy Networks).

Over the past few weeks, government IT staff have scaled up VPN access and network capacity as quickly as they can. It’s really impressive work, but one of the questions is **why government network and remote access capacity was so constrained to begin with**. It’s likely a combination of a few things: old buildings without modern network cables and switching equipment; old (basement) data centres that were already slated for upgrades; a limited number of licenses for VPN software that work on a per-connection basis (either on the client or server side); not enough server capacity to handle remote desktop or VPN connections.

There’s another limiting factor, though: **the dedicated security hardware used in corporate networks across government**. These are hardware-based firewall and network monitoring devices ([F5 hardware devices](https://www.f5.com/products/big-ip-services/iseries-appliance), for example) designed to observe all of the traffic going in and out of the “perimeter” of corporate networks. This is normal in government institutions, banks, and other large companies – and it’s also one of the main reasons why scaling up bandwidth and remote access is so difficult.

A colleague asked me once if it was legal for our department’s IT security folks to monitor our internet traffic. Formally, for Canadian government employees, your department is [required to let you know](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=32607) that “electronic network monitoring practices” are being applied (and if you’re connecting through a corporate network or VPN, they are); typically that’s part of the acceptable use screen that you consent to before you log into your corporate device. Spoiler alert, it’s legal.

[Alex Stamos](https://twitter.com/alexstamos) (previously the VP of security at Yahoo, then CSO at Facebook, and now a professor at Stanford) gave a great overview of why perimeter network monitoring is a problem [in a 2015 keynote at the OWASP security conference](https://www.youtube.com/watch?v=2OTRU--HtLM). It’s a long presentation, but worth watching. One of the takeaways is that, for companies and organizations operating at scale, it’s becoming a “completely ridiculous idea” to buy security hardware. These monitoring devices are the slowest and most energy-intensive pieces of any data centre operation, and they [don’t work well with the containerized, automatically-scaling model](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-190.pdf) of modern, cloud-based software infrastructure. 

To networking and IT security staff that have been working on corporate networks for a long time, this probably seems sacrilegious. Network perimeter monitoring (through the enterprise firewall devices that Alex Stamos criticizes in his talk) was long one of the main tools used to watch for unauthorized or unexpected traffic, hacking attempts, or compromised devices. Moreover, the hundreds of legacy applications on the inside of the corporate network typically have almost no application security features whatsoever – what my friend [Mike Williamson](https://twitter.com/dexterchief) calls the “crunchy outside, gooey inside” approach to IT security (this approach is …no longer a best practice).

I’m not advocating that departments get rid of their corporate networks tomorrow, or unleash the world upon their undefended legacy applications. But as organizations (government departments included) plan what they need for the future, it’s clear that corporate networks and the dedicated security hardware guarding the perimeter aren’t it. The main downsides, in a “[cloud-first](https://www.canada.ca/en/government/system/digital-government/modern-emerging-technologies/cloud-services/government-canada-cloud-adoption-strategy.html#toc6)” world are:

*   putting security hardware that _can’t_ scale well as a chokepoint between end-users or staff and cloud-based applications and services, which _do_ scale well

*   introducing single points of failure (the security hardware itself, and/or on-premise remote desktop or VPN servers) that are liable to fail when you need them most

*   adding significant complexity when new cloud-based services need to connect “into” the corporate network to talk to a legacy system (particularly in the Canadian government, in which this automatically introduces an external dependency on networking staff from Shared Services Canada)

*   creating a false sense of security and diverting investments away from application security and other modernization efforts

This isn’t a uniquely Canadian problem, but other governments are taking proactive steps to move away from corporate networks. The United Kingdom announced in 2017 that they would [officially begin moving away from their Public Services Network (PSN)  corporate network](https://governmenttechnology.blog.gov.uk/2017/01/20/the-internet-is-ok/):

> At a recent meeting of the Technology Leaders Network, we reviewed our position and it was clear that everyone agreed we could just use the internet.

> From today, new services should be made available on the internet and secured appropriately using the best available standards-based approaches. When we’re updating or changing services, we should take the opportunity to move them to the internet.

**The future is the regular internet**. Moving away from corporate networks isn’t easy; there’s a lot of path dependency from previous investments, previous security policies and approaches, and (in Canada) from the organizational history of departments like Shared Services Canada (that reinforce a divide between networking and sysadmin staff, in SSC, and application developers in individual departments). 

Investing more in modern application security and building cloud-native applications is an important first step; large-scale cloud providers have a range of audit logging and monitoring features built into their service offerings that mitigate the need for separate firewall devices.

Avoiding any requirement for these applications to pass through or depend on corporate networks is the second step. Google’s [“zero-trust” security model](https://cloud.google.com/beyondcorp) – assuming every device might be compromised, and engineering secure systems with that in mind – is a good example of what this future path can look like. 

Right now, federal government employees are largely all working from home, using online tools (like Office 365) that are also off the corporate network. It raises the question: what value is a perimeter when everything is outside it?

I’ll end off with [a presentation](https://www.youtube.com/watch?v=a4UXnZaunJQ) from the US Digital Service’s [Marianne Bellotti](https://twitter.com/bellmar) at the 2017 Strangeloop conference, on her work to remove US government requirements for “Trusted Internet Connections”. Security policies that make it harder to build modern, reliable, and scalable software ultimately end up making things less secure.

{{< youtube id="a4UXnZaunJQ" class="youtube-embed" >}}

_Thanks to [Mike Williamson](https://twitter.com/dexterchief) for the conversations that inspired this post._
