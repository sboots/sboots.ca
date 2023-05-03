---
title: "“Fake COTS” and the one-day rule"
date: 2020-09-16T18:38:13-07:00
summary: "One of the long-held norms of government IT is the perceived benefit of “commercial, off the shelf” software solutions. In government environments, being able to buy ready-to-go software products to meet government IT needs is appealing. In many cases, though, extensive customization requirements means that COTS purchases don’t live up to their promise. They’re marketed as a car and they turn out to be boxes of car parts: lots of time-consuming assembly required. Here’s a rule of thumb to tell the difference between genuine and fake COTS."
extradisclaimer: "The views expressed here are my own. Products mentioned in the examples below are not endorsements."
images: ["/img/2020/whitehorse-empty-pandemic-shelf.jpg"]
featured: true
---

One of the long-held norms of government IT is the perceived benefit of COTS solutions: “commercial, off the shelf” software. In government environments where IT [isn’t seen as a core competency](/2020/05/20/the-cycle-of-bad-government-software/), and that by and large are [short on technical expertise](/2020/05/26/why-are-there-so-few-senior-developers-in-government/), being able to buy ready-to-go software products to meet government IT needs is an appealing approach.

COTS software has a number of benefits, in a government setting:

*   It’s potentially ready to use right away
*   There are existing customers, so you’re not dealing with the bugs or issues that come with the first version of a product
*   You’re paying for a commercial product (software licenses, for example), rather than hiring staff or contractors to build something (which introduces a range of complex HR or project management steps)

Various Government of Canada guides over the years speak highly of COTS approaches: “Acquire commercially available items [unless custom-made items are essential to operational requirements](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=14671)” and defining COTS as “commercially available products that can be purchased and integrated with little or no customization, [thus facilitating customer infrastructure expansion and reducing cost](https://www.tbs-sct.gc.ca/pm-gp/doc/pcrag-ecrpg/pcrag-ecrpgpr-eng.asp).” Some government standards written in the early 2010s [require specific COTS products for particular business processes](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=25687) (PeopleSoft and OpenText Content Server are two examples of this).

The appeal of COTS products is essentially: if you have the same need as someone else, and a widely-used commercial product exists, why not use it? That way you can spend your time and resources focusing on the unique aspects of what you do, rather than reinventing the wheel. 

Seems rosy so far, right? Here’s the catch…

## A car versus a box of car parts

Almost all software solutions marketed at government institutions are described as COTS products. Calling your product a COTS solution is a key part of government IT sales and marketing. What happens as a result is that a lot of COTS-branded software products don’t live up to that “off the shelf” label:

Any software product needs setting up, configuring, or tweaking to make it useful for a given goal. But the amount of customization required to make a COTS solution useful is what distinguishes genuinely-useful COTS software from “fake COTS”, that’s off-the-shelf in name only. 

In 18F’s (fantastic) [De-Risking Guide](https://derisking-guide.18f.gov/), the team [writes](https://derisking-guide.18f.gov/federal-field-guide/#consider-tradeoffs-in-build-or-buy-decisions-taking-all-factors-into-consideration):

> Government agencies often describe challenges and the expense of customized commercial off-the-shelf (COTS) software. These efforts often start out as a pure COTS implementation, until agencies realize that they need to customize the software to meet their needs. 
> 
> In these situations, the agency pays industry to develop custom software that the agency may end up locked into, especially if, as often happens, the agency did not secure sufficient data rights in its contract. 
> 
> Over time, these systems become more difficult to maintain, as new features and customizations are added to the base COTS product, each of which bring it further away from actually being COTS. 18F technologists often refer to these products as “unrecognizably modified off-the-shelf” software, or “UMOTS.”
> 
> **Modifying COTS software eliminates most of the benefits of using COTS.** Customized COTS is often modified to the point where routine software updates can no longer be applied. At this point, the software requires expensive custom updates for the duration of the software’s life. It also locks the agency into a long-term (and often sole-source) relationship with that contractor.

How do you tell how much customization is too much? This is a frequent challenge for government organizations without the in-house technical expertise to be able to see through the marketing claims vendors make about their products. 

Some COTS products are genuinely solutions you can adopt and use quickly. **Other COTS-branded products are the equivalent of ordering a new car, and instead getting a large box of car parts.** In theory, you got a car, but it’ll take years and a lot of specialized expertise before you can use it. (Without enough specialized expertise on hand, you might never end up with a car at all.) You might’ve even received the parts [to build a truck or a minivan instead](https://18f.gsa.gov/2019/03/26/when-to-use-COTS/), if you wanted to, but if you were hoping to drive it tomorrow, you’re out of luck.

## The one-day rule

How do you tell the difference between genuine and fake COTS? When every piece of software needs to be configured at least a little bit, how much customization is too much? 

Here’s my personal rule of thumb: 

*   If you can get a software solution to successfully meet your needs **in one day**, it’s a real COTS product. 

Yes: one normal work day, with one or two people and a reasonable but not extravagant level of technical expertise. **If it takes longer than that, it’s fake COTS.**

There’s two side cases that I’ll allow: 

*   You get an extra day, if you need it, to figure out how to deploy the software solution across a set of managed devices (e.g. corporate software deployments). 
*   And, you get an additional extra day to figure out how to bulk import data that’s been exported from whichever solution you were using before. (Time spent getting the data _out_ of the previous system doesn’t count, since it’s not the new system’s fault!) 

If both of those apply, you get three days and you can still call it a genuine COTS solution. 

## Examples

Let’s see what that looks like in practice! You can probably see this coming – most online software-as-a-service products do this really well (one of the reasons why the Canadian government’s [Cloud Adoption Strategy](https://www.canada.ca/en/government/system/digital-government/digital-government-innovations/cloud-services/government-canada-cloud-adoption-strategy.html#toc6) prioritizes them), as do software products aimed at regular, non-government consumers. Government-oriented COTS products largely all fail to live up to the one-day rule.

### How long it takes to purchase and get a software product working 

Under one day (all times are anecdotal, your measures may vary):

*   [Microsoft VS Code](https://code.visualstudio.com/): 10 minutes
*   [Trello](https://trello.com/en): 15 minutes
*   [Slack](https://slack.com/intl/en-ca/) for a small or medium team: 15-30 minutes
*   [GitHub](https://github.com/) for a small team: 20 minutes
*   [SurveyMonkey survey](https://www.surveymonkey.com/): 20-40 minutes
*   [DigitalOcean instance](https://www.digitalocean.com/): 30 minutes
*   [Amazon RDS database](https://aws.amazon.com/rds/aurora/): 30-45 minutes
*   [Google G Suite](https://gsuite.google.ca/intl/en_ca/) for organizations: 1 hour (plus an available domain name)
*   [Adobe Creative Cloud](https://www.adobe.com/ca/creativecloud.html): 1-2 hours depending on internet bandwidth (for individual use; government purchases via standing offer are 3-6 months)

Over one day:

*   [Oracle PeopleSoft](https://www.oracle.com/ca-en/applications/peoplesoft/): 4-6 years
*   [OpenText Content Server](https://www.opentext.com/products-and-solutions/products/enterprise-content-management/content-management) (GCdocs): 2-4 years
*   [Microsoft Dynamics CRM](https://dynamics.microsoft.com/en-ca/): 1-2 years
*   [Adobe Experience Manager](https://www.adobe.com/ca/marketing/experience-manager.html): 1-3 years

You can see examples of various implementation projects using these solutions and their timeframes in the [list of large Government of Canada IT projects](https://large-government-of-canada-it-projects.github.io/), by searching for them in the search field for a given year’s data.

All of these government-oriented products, it’s safe to say, are boxes of car parts: time-consuming assembly required. If you have teams of developers and several years to turn them into the product you actually want, go for it. If you want something that’s ready to use, right off the shelf, they’re not good choices.

## The simplicity is the point

If you’re a grizzled government IT veteran, reading this you may immediately think: how naïve, how simplistic; government needs are just inherently complex and it’s unavoidable for projects with complex requirements to take this long.

To which I would say, that’s fine ([except it isn’t](/2020/02/25/our-services-arent-working/)). The point here is that, if “off the shelf”-branded solutions take several years to implement, which in government [they consistently do](https://www.cbc.ca/news/canada/ottawa/phoenix-federal-government-report-lessons-1.4339476), then the “off the shelf” label means very little. 

The one notable caveat in the examples above is that most of the “under one day” products above are tools for individuals, while the “over one day” products are tools for business processes. Business processes (like delivering various kinds of government services) aren’t things that you can figure out in a day; they take [research and thoughtful design and iterating over time](/2020/02/27/user-needs-not-government-needs/). That’s fine! But that’s also partly the point: no “off the shelf”-labelled product will single-handedly make a complex business process work, which is why the COTS label in a government IT context feels so disingenuous. 

If you’re [designing a government service](/2020/06/16/building-digital-services-in-the-canadian-government/) over the course of several months, starting with a COTS-branded product (particularly those marketed at government, not consumers or regular companies) instead of something built in-house isn’t likely to save much time anyway. It could just as likely slow implementation teams down by having to work with a “[one size all fits nothing well](/2020/02/04/perils-of-standardization/)” product as a starting point, rather than open-source components that are free, much simpler, and easier to work with. (And, if your data, business rules, or requirements are complex enough that your IT project really will take several years to implement, it’s [probably doomed to failure from the start](https://waldo.jaquith.org/blog/2020/02/stop-procurement-failures/).) 

COTS is a marketing term, not a technical term. It’s a branding term that says: you can use this right away. The one-day rule is a simple way to call that bluff, across a wide range of types of software products. If you want to buy a car, and drive it this week, don’t buy a box of car parts. 

_I love bicycling and so using this car-buying metaphor feels weird – but after [moving to Whitehorse](/2019/12/17/moving-to-the-yukon/) we leased a Subaru Crosstrek and, turns out, it’s …really really great._
