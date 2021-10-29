---
title: "Rule number one: Avoid vendor lock-in"
date: 2021-05-12T16:07:26-07:00
summary: "If you’re working on IT or service delivery projects in public sector organizations, I have one very specific rule for you to follow: avoid vendor lock-in. To do that, you should own your data, own your front-end interfaces, own your software source code, and avoid long-term contracts. This post dives into why vendor lock-in is a problem, and how those strategies can help prevent it."
subtitle: "Rule number two: see rule number one"
extradisclaimer: "Views expressed here are my own, and don’t necessarily reflect the views of the Government of Canada. Products mentioned below are examples and not endorsements."
images: ["/img/2021/saskatoon-highway-exit.jpg"]
---


People who know me know that I’m not a big fan of rules. My [day job](https://digital.canada.ca/2018/09/07/policy/) involves a lot of navigating and working around outdated rules, helping teams figure out which rules are [red rules instead of blue rules](https://eriemeyer.medium.com/user-research-is-not-illegal-uncle-sam-51f2f92a280a), and trying to change existing rules to be more empowering to digital service delivery teams and everyday public servants. Interpretations of rules and myths around them are [some of the main barriers](/2020/02/27/user-needs-not-government-needs/) to governments trying to adopt more modern ways of working.

On more than one occasion, friends who are working on rule changes (updated administrative policies, for example) have asked what I’d suggest, and my non-sarcastic answer has been: if we actually got rid of _all_ of those rules, would it lead to better outcomes?

I have one exception, though! My general advice for life is: be a good person, and care for the people around you. And follow this one very specific rule: **avoid vendor lock-in**.


## What is vendor lock-in?

Vendor lock-in is a situation that government and institutional IT teams often find themselves in, where they are dependent on a specific vendor (an IT systems provider, software company, or management consultant) and they aren’t able to stop using them. 

It’s a power dynamic where IT teams aren’t able to make changes (for example, to improve a system or move to a new one) because they’re stuck with their current vendor. It can happen for a variety of reasons, and it usually emerges over a period of time. 

**Vendor lock-in is a problem because it slows down or prevents teams from making improvements; it leads to worse user experiences over time, as a result; and it often leads to dramatically higher costs**. It’s great for vendors, though, who benefit from an always-increasing revenue stream and a guaranteed customer, no matter the quality of the product or service they’re offering.


## How do you avoid vendor lock-in?

Have an exit strategy! **Avoiding vendor lock-in is all about finding ways to keep your future options open**. There’s a great quote [from one of the original writers](https://pragdave.me/blog/2014/03/04/time-to-kill-agile.html) of the [Agile Manifesto](/2020/01/28/introducing-agile-to-large-organizations-is-a-subtractive-process-not-an-additive-one/): 

> When faced with two or more alternatives that deliver roughly the same value, take the path that makes future change easier.

The suggestions below are strategies to avoid vendor lock-in, and to [preserve your ability to make future changes](/2021/02/14/if-you-want-enterprise-services-to-be-good-make-them-optional/). They’re written for public service teams working on technology and service delivery projects. Some of these strategies depend on a certain level of internal technology capacity – something organizations [aren’t always prepared for](/2020/05/26/why-are-there-so-few-senior-developers-in-government/), but that over time is likely cheaper than a locked-in dependence on an external vendor. In other cases, these can be achieved simply by writing better procurement contracts with the vendors you work with.

It’s a long post! Here’s quick shortcuts to each section:

1. [Own your data (and make sure you can move it somewhere new)](#1-own-your-data-and-make-sure-you-can-move-it-somewhere-new)
2. [Own your front-end interfaces](#2-own-your-front-end-interfaces)
3. [Own your software source code](#3-own-your-software-source-code)
4. [Avoid long-term contracts](#4-avoid-long-term-contracts)

And lastly, since I’m sure you’re wondering: [What should vendors do, then?](#what-should-vendors-do-then)

### 1. Own your data (and make sure you can move it somewhere new)

The biggest mistake I see in past government procurements is not explicitly owning the data generated, input into, or collected by a vendor-operated system. This can include user account data, case management information, documents, financial records… all the things that, if you were to switch from your current vendor’s system to a competitor’s system, you’d have to somehow extract and move. If you as an organization don’t actually own that intellectual property, then you’d need to start from scratch in order to change vendors. 

In worst-case scenarios, I’ve heard of cases where organizations have had to bargain or plead with their current vendors to give them this data, prior to running a competitive procurement process for a replacement system _that the same vendor will be participating in_. It’s not a bargaining position you want to be in. Lock it in to the very first contract you write, that you as the government or organization own the data (including user account information) that will be stored in the system.

Even if you own the data, actually getting it out of a system in a format that can be re-used is also frequently a problem. Older proprietary databases, case management systems, and enterprise resource planning systems often didn’t have any systematic way to export data. Without built-in, comprehensive export features, migrating to a different system becomes a manual, error-prone, and potentially years-long process.

As a rule of thumb: **have an exit strategy written down for any major system before you even start using it**. (Can you export all of the data the system stores, in an automated, machine-readable way? That’s the bare minimum.) Your future self, years later, will thank you.

<figure>
  <img src="/img/2021/saskatoon-highway-exit.jpg" class="img-fluid" alt="A photo of a highway overpass and offramp in Saskatoon, taken from the passenger seat of a car. The highway sign above says, “Circle Drive” ahead, “Central Avenue and College Drive East MUST EXIT” to the right">
  <figcaption><span class="sr-only">Caption: </span>Always have an exit strategy.</figcaption>
</figure>

### 2. Own your front-end interfaces

Interfaces refers to [the way that people interact with your service or system](/2020/10/19/interfaces-data-and-math/#interfaces) – what it looks like, how it works, and how people use it. “Front-end” refers to the layer that people see (for example, the website or web application that they directly interact with). 

Interfaces can be challenging to build and maintain, and it takes a lot of expertise [to make user-friendly and accessible services](/2020/06/16/building-digital-services-in-the-canadian-government/). External vendors are often hired to build and maintain these interfaces, as a result. 

In many cases, however, organizations will simply outsource an entire service to an external vendor. This sets up a situation where people interact with the vendor’s website and interfaces directly, instead of with the organization itself. This intermediary role and function – one that places a vendor between a government and the people it serves, is one to be protected and managed extremely carefully. There’s a strong argument to be made that front-facing service delivery functions like this should never be outsourced. How this shows up in new procurements is an area to keep a close eye on. 

The vendor lock-in here comes from the fact that, over time, people using the external vendor’s service will get used to it. People **identify the vendor and their products as the way to receive a given public service**, rather than the public sector institution that is now behind the scenes. That makes it disruptive and complicated to switch to an alternative service (either in-house or from a competing vendor). Or at the least, it will feel prohibitively disruptive to decision-makers in your own organization, who will want to stick with the existing vendor longer than it adds value. One way to think about this is as self-constructed lock-in – even if you can legally end the contract, can you functionally expect people to stop using it? Likewise, from the inside of the public sector organization, once established operational workflows are built around a specific product they create a significant disincentive for future change. Habits and routines make changing later all that much more difficult. 

Even if your organization doesn’t have in-house expertise in front-end interfaces, you can hire a vendor to build high-quality services that you own and operate (more on that below). If your approach instead is just to deliver services that aren’t user-friendly, that’s [not a great solution](/2020/02/25/our-services-arent-working/#a-lack-of-focus-on-end-users).

One last part of owning your front-end interfaces is **owning the domain name or subdomain that a service is running on**. If a vendor helped you set it up but they own the domain name registration, then there’s no way to move away from that vendor without either forcing people to learn a new website address for your service, or having that vendor cooperate nicely in your own departure. Don’t count on the latter. 

### 3. Own your software source code

Governments and organizations depend on a lot of custom software code, whether it originates from purpose-built systems or [customizations to “commercial, off the shelf” software](/2020/09/16/fake-cots-and-the-one-day-rule/). In the Canadian federal government, most of this software code is written by external contractors.

Historically, a lot of this software code has been owned by these contractors; various administrative policies [encourage this](https://www.ic.gc.ca/eic/site/068.nsf/eng/00005.html). Even software that was originally developed in-house by government institutions has been spun-off into commercial software companies, [through processes established for this purpose](https://www.tbs-sct.gc.ca/pubs_pol/opepubs/tb_b4/ett01-eng.asp), only for the government to then pay to license it back from those companies. 

All this is to say: Canada is pretty late to [the open source approach](/2020/08/20/make-things-open-source-it-makes-things-better/) that other governments [enthusiastically adopted years ago](/2019/12/26/suggestions-for-the-next-gc-cio/#medium-term). 

When you don’t own your software source code, you’re vulnerable to vendor lock-in in a few ways. The licensing terms for a software product might prevent you from making certain kinds of modifications or improvements (including, for example, changes that would make it easier to export data). Modifications that you’ve made over time, built into or using the same proprietary software products and languages, can make migrating to a replacement system feel even more complex and unattainable. 

Not even considering proprietary software licensing costs, all of these are reasons to own the custom software source code you depend on. When you’re starting a new project, using open source software products as a foundation, or existing software that you already own, is a critical way of avoiding long-term vendor lock-in. Making your own custom software code open source, so it can be [shared and re-used by other organizations](/2020/08/20/make-things-open-source-it-makes-things-better/), is also a big win for both financial stewardship and public transparency.

As [Bianca Wylie](https://twitter.com/biancawylie) would say: [public money? Public code](https://web.archive.org/web/20210513170516/https://twitter.com/biancawylie/status/1388692375665618950).

### 4. Avoid long-term contracts

There are a lot of incentives for public servants to set up long-term contracts, and the [onerous nature of government procurement processes](https://policyoptions.irpp.org/magazines/february-2019/outdated-procurement-rules-hindering-digital-government/) is one of the biggest ones. (Waterfall-oriented budget and planning approval cycles are others.) Undertaking a complicated procurement process every few years isn’t appealing, and so public servants often set up five- or seven- or ten-year long contracts with IT vendors and service providers.

Fight that temptation. Long-term contracts are vendor lock-in _on purpose_; the other sources of vendor lock-in above (not owning your data or interfaces or source code) are vendor lock-in by accident.

Among digital transformation types, you’ll often see everyone shaking their heads as yet another government department celebrates successfully signing a ten-year contract with an IT vendor. **The only constant in the technology world is change.** What your needs are, as a government institution, will be dramatically different a decade from now. (If they aren’t, you probably aren’t serving your constituents or service users as well as you should be!) The products or services a given vendor provides, even if they’re the best-in-class today, aren’t necessarily going to be the best, cheapest, most secure, or most accessible in a decade. 

When you’re putting together a procurement contract, keep your options open by keeping the contract length as short as you possibly can. Two years is alright; three years is long; anything longer and you’re setting yourself up for future embarrassment. If you’re working with a complicated system or you’re really constrained for technology talent, then a two- or three- year contract with a few option years afterwards might be okay. Don’t lock yourself in to anything longer than that.

Countries that are further ahead in their digital transformation journeys have implemented [maximum monetary value and duration limits on IT contracts](https://webarchive.nationalarchives.gov.uk/20170909132908/https://www.gov.uk/government/publications/technology-code-of-practice/technology-code-of-practice). In the future, it would be [great for Canada to adopt a similar approach](/2019/12/26/suggestions-for-the-next-gc-cio/#long-term).

## What should vendors do, then?

This post might seem like it’s setting IT vendors up as some kind of villain; they’re not, they’re just responding to the incentives that exist for them in public sector IT. (If you’re a vendor, I’m sure you’re cool!) 

By becoming a more savvy, vendor lock-in-aware customer, you’re incentivizing the vendors you work with to put forward their best work. If you’re able to easily switch to another vendor whenever the situation warrants, your vendors will be that much more motivated to do high-quality work.

There’s a few areas where using an external vendor often does make more sense than doing things in-house. These include:

*   **Public cloud infrastructure**. Large-scale cloud providers like [Amazon Web Services](https://aws.amazon.com/), [Microsoft Azure](https://azure.microsoft.com/en-ca/), and [Google Cloud Platform](https://cloud.google.com/) offer highly reliable, secure hosting and computing services at a much lower cost than bespoke, on-premise systems. The Canadian government [recommends public cloud](https://www.canada.ca/en/government/system/digital-government/digital-government-innovations/cloud-services/government-canada-cloud-adoption-strategy.html#toc6) for practically any use-case (outside of defense and intelligence work). As a government institution, you should manage accounts on cloud infrastructure yourself, rather than depending on a third-party vendor or reseller to do this. There _are_ some [important philosophical issues](https://thereboot.com/the-infrastructural-power-beneath-the-internet-as-we-know-it/) with large-scale cloud providers, but my main reason to recommend them is that you can [begin using them very quickly](/2020/09/16/fake-cots-and-the-one-day-rule/#examples) – in minutes, not days or months (compared to many governments’ internal shared or cluster infrastructure options). These large-scale cloud providers are inexpensive and high quality. And as long as you manage the accounts yourself and own your own domain names, you could switch from whichever cloud provider you’re using to a competitor whenever you want to.

*   **Specialized behind-the-scenes services**. API-based platforms like [Twilio](https://www.twilio.com/) (for SMS and phone communications) and [Stripe ](https://stripe.com/en-ca)(for credit-card handling) have great reputations for reliable service delivery and easy integration into other systems. (Part of this is thanks to high-quality developer documentation). You can integrate these platforms into your services while still owning your front-end interfaces and the rest of your software source code. In areas like credit-card handling that have [stringent security compliance requirements](https://en.wikipedia.org/wiki/Payment_Card_Industry_Data_Security_Standard), offloading this to a vendor like Stripe can significantly reduce the complexity of your service. As always, just make sure you have an exit strategy to another provider if you end up needing it.

*   **Custom software development, if you really need to (but open source it!).** Many government institutions don’t have the in-house design and technology talent needed to deliver modern online services. That’s [a significant problem](/2020/05/26/why-are-there-so-few-senior-developers-in-government/), but in the short term, depending on vendors is going to be a reality for most organizations. To do this well, in a way that avoids vendor lock-in, there’s three steps to take. The first is, require that the intellectual property developed under the custom software development contract is owned by your organization (for example, the Government of Canada). The second is to license that custom software [under an open source license](/2020/08/20/make-things-open-source-it-makes-things-better/) and to publish it publicly somewhere (ideally, in real-time as it’s built by the vendor). The third is to keep the contract for custom software development fairly short (again, two to three years) so that, if need be, you can switch to a competing vendor in the future. [As long as the software code is owned by your organization and publicly published](https://waldo.jaquith.org/blog/2020/08/make-sure-your-ui-modernization-plan-includes-an-open-source-clause/), the replacement vendor can then fairly seamlessly continue working on the software initially produced by the first vendor. As an added benefit, the vendors involved will be [motivated to do high-quality work](https://gds.blog.gov.uk/2017/09/04/the-benefits-of-coding-in-the-open/), since it can be scrutinized by the entire world. 

*   **External security and accessibility audits.** There are some areas of design and technology where specialized expertise can be particularly critical. Making sure that your services are secure and robust – and [making sure that everyone can use them](/2020/06/16/building-digital-services-in-the-canadian-government/#accessibility) – is essential. Even if you have in-house technology capacity, it can often be really helpful to enlist an external provider for security and accessibility reviews, especially at certain points (prior to launching a brand-new or redesigned service, or a large-scale new feature). Over time, you should develop in-house security and accessibility expertise, but short-term contracts with companies that specialize in these fields can be a lifesaver in the meantime.

Vendor lock-in doesn’t just happen in government institutions; it can happen in private companies as well. But it seems to be extra prevalent in public sector organizations, partly (in my view) because of how laborious approval and contracting processes are; partly because of [outdated IT strategies](/2020/02/04/perils-of-standardization/); and partly because of [a lack of technology expertise among senior decision-makers in the public service](/2020/05/20/the-cycle-of-bad-government-software/). This is compounded by situations where government departments and public service leadership _depends on vendors for advice on how to deal with vendors_. (This frequently occurs with management consulting companies, who also have large IT service provider divisions.) I’ll write more about these in future posts.

Thanks for reading! Thoughts and feedback are always welcome, [don’t hesitate to reach out](https://twitter.com/sboots) anytime!

_Curious what vendor lock-in looks like in a tangible way? Read about the City of Toronto’s recent PayIt procurement in [Regs to Riches](https://www.regs2riches.com/p/-pay-what) and [Tech Reset Canada](https://www.techresetcanada.org/not-another-presto)._
