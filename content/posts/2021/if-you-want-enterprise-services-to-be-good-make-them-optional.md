---
title: "If you want enterprise services to be good, make them optional"
date: 2021-02-14T20:52:15-07:00
summary: "Enterprise IT systems in government are often enforced as mandatory solutions that other teams and departments are required to use. In comparison, leading tech companies turn their internal systems into external products, to see if they are commercially viable. Making enterprise services optional creates feedback loops, generates adoption-rate data, and incentivizes continuous improvement."
images: []
---

“Enterprise” is a fascinating term, in that it’s widely (and aspirationally) used in government and organizational IT, and also [made](https://twitter.com/waldojaquith/status/709890615765549056) [fun](https://twitter.com/allenholub/status/1349842056852738049) [of](https://twitter.com/kelseyhightower/status/1359176847481708545) frequently by digital transformation advocates. Generally speaking it means: systems and services that are used across an entire organization, rather than just one specific program or team. In government settings, “enterprise” often means services that are used across the entire government, or, efforts to make that a reality.

I’ve written before about [how standardization efforts often backfire](/2020/02/04/perils-of-standardization/), and it’s one of the reasons that enterprise IT systems – standardization on as large a scale as possible – tend to have a bad reputation. 

As a concept, adopting enterprise approaches is [a fairly widely-held priority](https://www.canada.ca/en/shared-services/ssc-3-enterprise-approach.html) in the Canadian government. Fewer systems, adopted more widely, can mean less specialized training and expertise is necessary, and that staff can move from team to team or organization to organization without having to re-learn how unique systems work. In [an expertise-constrained environment](/2020/05/26/why-are-there-so-few-senior-developers-in-government/), this isn’t a bad approach. But there’s an (admittedly counter-intuitive) way to significantly increase the quality of enterprise systems: make them optional.

## An Amazon case study: if you don’t have competition, create it

Amazon (yes, the online bookstore-turned-logistics and software behemoth) is famous for its approach to software engineering. David Eaves has [a great article about Amazon’s engineering approach here, and what it means for government IT](https://fcw.com/blogs/lectern/2017/05/no-more-systems-integrators.aspx). A simple software architecture decision in the early 2000s – that any internal services need to be externalizable, and to communicate with each other using [APIs](http://101.apievangelist.com/) – laid the groundwork for what became Amazon Web Services, the largest cloud infrastructure provider operating today.

By building internal systems with the scalability and security that would let them be adopted by the outside world, it was easy for Amazon to turn its internal infrastructure into services that other customers could pay for and use.

There’s a more subtle benefit to this approach, beyond just being able to make money from surplus computing power. **By turning its internal systems into external products, Amazon can very quickly learn if its internal systems are commercially-viable.** If they’re not, then Amazon can either invest in improving a given internal system, to catch up to whatever competitors exist in that field, or they can drop it and use a competing product internally instead. 

At [my old company](https://viamo.io/), we built communications and survey tools used by international development organizations. One of the optional services we provided was setting up or helping operate small call centres. In 2017, Amazon launched a self-service call centre platform, which we watched with a lot of interest. Having Amazon launch a product in your field is …not an uncommon experience for tech start-ups. 

One of the reasons Amazon launched this product was **to see if their own internal call centre software was good enough** to keep using it. As [a TechCrunch article from the time explains](https://techcrunch.com/2017/05/14/why-amazon-is-eating-the-world/?guccounter=1):

> In the 10+ years since AWS’s debut, Amazon has been systematically rebuilding each of its internal tools as an externally consumable service. A recent example is AWS’s Amazon Connect — a self-service, cloud-based contact center platform that is based on the same technology used in Amazon’s own call centers. Again, the “extra revenue” here is great — but the real value is in honing Amazon’s internal tools.
> 
> If Amazon Connect is a complete commercial failure, Amazon’s management will have a quantifiable indicator (revenue, or lack thereof) that suggests their internal tools are significantly lagging behind the competition. **Amazon has replaced useless, time-intensive bureaucracy like internal surveys and audits with a feedback loop that generates cash when it works — and quickly identifies problems when it doesn’t.** They say that money earned is a reasonable approximation of the value you’re creating for the world, and Amazon has figured out a way to measure its own value in dozens of previously invisible areas.

## “Mandatory” is not the advantage you may think it is

If you’re someone providing an enterprise service in government – whether it’s Government-as-a-Platform products, internal IT systems, web services, infrastructure, or anything else – you might be tempted to make it mandatory.

In government IT settings, decision-makers make particular internal software products or systems mandatory all the time. I’m curious why this happens, and I think it might be in part because – for public servants in leadership roles – making a thing mandatory [seems more concrete and decisive](/2020/02/04/perils-of-standardization/#a-placeholder-for-more-informed-technical-discussions) than making it optional. In an environment where successful outcomes are long-term and hard to measure, simply making a clear decision is seen as a metric for success. Accurately tracking the long-term costs of IT projects and systems is also something that governments struggle with, and having one single system instead of several intuitively _seems_ cheaper, even if that might not be the case in reality. 

When I think of the (mandatory) enterprise software solutions in place in the Canadian government – the [Phoenix pay system](https://www.cbc.ca/news/canada/ottawa/phoenix-pay-system-cost-could-total-2-6b-before-cheaper-replacement-ready-1.5138036), the [Shared Travel System](https://internal-red-tape-reduction-report.github.io/annex-2/#snapshot-the-trouble-with-travel), [GCkey](https://www.cbc.ca/news/politics/cra-gckey-cyberattack-1.5689106) to sign into websites, the [content management system that powers Canada.ca](https://www.cbc.ca/news/politics/canadaca-federal-website-delays-1.3893254), the Shared Case Management System, GCdocs, and a number of others – none of them are solutions that in good faith I’d recommend that friends and colleagues in the public service use, if they had the choice. I wonder if the fact that they are mandatory is actually one of the reasons why these solutions are as dated and [poor-quality](https://twitter.com/alexstamos/status/1338531560761409547) as they are.

In comparison – as the Amazon example above hints at – there are a number of clear advantages to building services that are optional:

*   **They create feedback loops.** Users can tell you why they chose to use, or not use, your product.
*   **They generate data about adoption versus competitors.** If users decide to use an alternative product instead, that can tell you volumes about what features or benefits are a priority for them.
*   **They incentivize continuous improvement.** If users have the choice to use other products, you’re motivated to keep on improving yours in order to retain them as a user.

These advantages all apply even without needing to worry about commercial viability, in government settings.

There are downsides to making enterprise services optional; they can lead to fragmentation and inconsistent user experiences. But I’d argue that there are more significant downsides to making poor-quality services mandatory. Government decision-makers have [a poor track record of telling the difference](/2020/05/20/the-cycle-of-bad-government-software/) between good- and bad-quality technology solutions. And, even if a product was the best choice at the time, the slow pace of government decision-making means that it’ll [still be mandatory](/2020/02/04/perils-of-standardization/#a-barrier-to-continual-change) five or ten years after it’s no longer the best option available.

If you’re a provider of enterprise software solutions, **your services should be good enough that people want to use them, even when they don’t have to**. And, from a professional craft and public service excellence standpoint: it’s better to build a good product that’s under-used than a bad product that’s over-used. Build good things, and make them optional. 
