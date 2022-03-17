---
title: "A bleak outlook for public sector tech"
date: 2021-12-15T20:34:17-05:00
summary: "Paul Craig recently wrote a blog post on the massive amount of compliance documentation his team produced to launch a small public website in a Canadian government department. It’s a must-read lens into the current shape of public sector tech work in Canada. We have a public service executive class that isn’t equipped to lead technology initiatives. We’ve got widespread adoption of digital government words, but not digital government implementation. And we’ve got a political class that is too busy with other things to care about the public service’s tech capacity. Let’s talk about it."
extradisclaimer: "The views expressed here are my own, and don’t represent the opinions of my team or my employer."
images: ["/img/2021/ottawa-office-boardroom.jpg"]
---

[Paul Craig](https://twitter.com/pcraig3) (one of the best developers I know) recently [wrote a blog post on the massive amount of compliance documentation](https://federal-field-notes.ca/articles/2021-12-15-paperweight/) his team produced to launch a small public website in a Canadian government department. It’s [a must read](https://federal-field-notes.ca/articles/2021-12-15-paperweight/):

> Traditional IT government projects try to guard against the possibility of costly mistakes by requiring product teams to seek approvals from a revolving door of committees and groups. Unfortunately, the accumulated time and energy spent appeasing these various gatekeepers can be just as costly to the team as the mistakes they are trying to prevent. In our case, our 12-page website needed approval from around 8 different groups over a 6-month period. … **For our 12-page site, we ended up writing almost as much as the Great Gatsby.**

> Something that was meant to optimize the team’s workflow and relieve a mild inefficiency turned into a black hole of effort: consuming hours and hours of time for documentation that few people will ever read.

> When the cost of trialling new things is so punishing, it is not practical or even rational to try. … I’m not saying we shouldn’t have _any_ compliance processes – of course we need security reviews and internal documentation of some kind. But above all we need procedures that are _proportional_ to the outcomes, that _adapt_ to changing situations.

This is a topic that’s near and dear to my heart, and one I’ve written about [a](/2020/06/02/blockers-versus-enablers/) [few](/2021/01/12/onerous-levels-of-oversight/) [times](/2020/01/28/introducing-agile-to-large-organizations-is-a-subtractive-process-not-an-additive-one/) [here](/2020/01/10/shipping/). 

Documentation is a good thing; done well, it helps new developers onboard to a project; it helps ensure that privacy and security approaches are shipshape; it’s a critical part of making interoperable software systems. But the vast majority of government IT documentation doesn’t actually do these things. 

If you work in a government IT operation, ask yourself how much time your team spends on building and [shipping](/2020/01/10/shipping/) software, and how much time it spends on what I call **“performative IT paperwork”**. What’s the ratio? There’s some minimal amount of paperwork (like the documentation examples above) that’s genuinely worth doing, but everything beyond that is taking time and resources away from actually meaningful work. (Which is to say: work that has [an impact on actual people](/2021/10/24/if-its-not-public-does-it-even-matter/).)

It’s comparable to the distinction [Mark Schwartz](https://twitter.com/schwartz_cio) (the former CIO of the US Citizenship and Immigration Service) makes [between “watching” and “doing”](https://twitter.com/honeygolightly/status/1224444073861242887). Most government IT organizations have vastly more people _watching_ (various project management, security, privacy, communications, enterprise architecture, IT standards, etc. roles and gatekeepers) than _doing_ (designers, researchers, software developers, DevOps staff, and product managers). And even then, organizational structures and processes mean that people ostensibly in “doing” roles end up [spending more time on “watching”-related activities](https://twitter.com/schwartz_cio/status/1388136215015215109). 

What’s unfortunate is that, in most government settings, IT organizations trend over time towards _more_ watching and less doing, because watching is easier and also [more similar to other government activities](/2021/01/12/onerous-levels-of-oversight/), which makes it more familiar and comfortable. That in turn makes “doing” [even more difficult](/2020/01/28/introducing-agile-to-large-organizations-is-a-subtractive-process-not-an-additive-one/).

The result? [Ten times more time and effort](https://federal-field-notes.ca/articles/2021-12-15-paperweight/#public-words) spent on performative IT paperwork than spent on building and shipping a useful product.


## Digital government: how are we doing?

Here’s where I’m at. **Public sector tech work (in Canada, at the federal level) is not in great shape.** This is a problem [for a bunch of reasons](/2020/02/25/our-services-arent-working/), but it’s a complicated one because it tends to be too niche for political leaders to care about, and too entrenched for grassroots public servants to be able to change (given the strong hierarchy of the federal public service). 

These aren’t the only factors involved, but they’re three that I’ve been thinking about a lot lately:


### 1. An ill-equipped executive class

The federal public service has about 80 deputy ministers and associated DMs, about 400 ADMs, and several thousand executives (in various director or director general/executive director -type roles). Several hundred public servants become executives for the first time each year:

{{< tweet user="APEX_GC" id="1460986878992207876" >}}

On average, I’d guess that it takes about 10 to 15 years between when someone joins the public service, and when they become an executive (with a lot of exceptions, for example people being recruited directly into executive roles, or joining the public service through programs like [RPL](https://www.canada.ca/en/public-service-commission/jobs/services/recruitment/graduates/recruitment-policy-leaders.html) that place them near the top of the non-executive classifications from the beginning). 10 to 15 years is a long time [to be inadvertently insulated](/2020/05/20/the-cycle-of-bad-government-software/) from how organizations work, and how technology is used, in fields outside of government.

Which is to say: of the 800 public servants that just joined the government’s executive ranks, **how many would be well-equipped to lead, champion, or shepherd a technology initiative?** My guess is, 20 or 30 of them, or less than 5%. How many will be _expected_ to lead or influence technology initiatives in some way? In all likelihood: _[all of them](/2020/11/16/government-is-actually-a-big-tech-company/)_.

(It’s also worth saying: those 20 or 30 tech-savvy public servants joining the executive ranks? That is _absolutely worth celebrating_, and they’re [going to have a positive impact](/2020/01/02/bridging-the-technology-policy-gap/) wherever they go in government. It’s just that there are so few of them, and that the senior executives still above them are likely to have skills and expectations that are yet more dated and insular.)


### 2. Agile words but not agile implementation

The second factor (and this comes up a lot lately in conversations with tech-minded public servants) is that, over the past few years, it’s become much harder to tell “who gets it” when it comes to digital government work. Digital-focused [teaching](https://www.csps-efpc.gc.ca/digital-academy/index-eng.aspx) [and](https://www.csps-efpc.gc.ca/tools/blogs/busrides/index-eng.aspx) [capacity-building](https://apolitical.co/digital-canada/) [efforts](https://www.canada.ca/en/government/system/digital-government/government-canada-digital-operations-strategic-plans/digital-operations-strategic-plan-2021-2024.html#toc06-4-1) (which, I should say, I’m a big fan of) have popularized the terms and ideals of digital government widely across the public service.

What that means, though, is: if you’re looking to work with government teams who are empowered and motivated to work in modern ways (and you should be), it’s now **much more difficult to tell those teams apart** from any other, more traditional, government IT team. 

If someone says “we use an agile process”, what used to be a vote of confidence is now a bit of a red flag:

{{< tweet user="PavelASamsonov" id="1468224595027181586" >}}

{{< tweet user="allenholub" id="1471907799416197120" >}}

Essentially: government IT teams have widely adopted the _words_ that fast-paced private sector tech teams use, without actually adopting their [ways of working](https://public.digital/2018/10/12/internet-era-ways-of-working). You virtually _can’t_ work in an iterative, user research-led, shipping-daily kind of way when you have to write 10 times more compliance documentation (as Paul [describes](https://federal-field-notes.ca/articles/2021-12-15-paperweight/#public-words)) than actual content and software code. 

The only solution [is to do less](/2020/01/28/introducing-agile-to-large-organizations-is-a-subtractive-process-not-an-additive-one/) of the performative IT paperwork long expected from established processes and gatekeepers, and that’s [a change to organizational power dynamics](https://twitter.com/worldofabe/status/1468291449896816644) [that can’t happen from the bottom](https://twitter.com/quidampepin/status/1445720169641357314). It needs to come from the top.


### 3. A pervasive lack of urgency

Given all this – and given that robust technology implementation is a requirement for any modern public service initiative – what might be the most disappointing is that **these issues don’t seem to be on the radar** of senior public service officials or of political leaders and parliamentarians. Promising steps [to emphasize digital government work at the ministerial level have been discontinued](https://policyoptions.irpp.org/magazines/november-2021/speaking-tech-to-power/). Public service renewal, or reform, or transformation – which is what digital government work [ultimately consists of](https://public.digital/definition-of-digital) – isn’t a high-priority topic of conversation anywhere.

_(Update: Mandate letters for ministers were published the day after I wrote this, [including one for the President of the Treasury Board](https://pm.gc.ca/en/mandate-letters/2021/12/16/president-treasury-board-mandate-letter) that includes a number of valuable digital government commitments. All told I’m feeling a bit more optimistic than a week ago.)_

In the United States, to contrast, investing in modern public sector tech is [an active, urgent effort](https://www.nytimes.com/2021/11/24/technology/government-tech.html). US departments are investing in [a number of](https://digitalcorps.gsa.gov/) [new ways](https://techtalentproject.org/) [to bring digital talent](https://twitter.com/_loganmcdonald/status/1453124547134300164) [into the public service](https://twitter.com/GSA_DaveZ/status/1432380570382778382). The Biden administration [has made reducing administrative burdens](https://twitter.com/donmoyn/status/1463153671928258560) [a public service-wide priority](https://www.whitehouse.gov/omb/briefing-room/2021/12/13/using-technology-to-improve-customer-experience-and-service-delivery-for-the-american-people/), to make it [easier for people](https://twitter.com/allafarce/status/1470777322454372359) [to access government programs and services](https://gen.medium.com/not-so-magic-words-why-im-still-excited-about-president-biden-s-new-executive-order-on-customer-4ba868eb5d2c). Civic tech luminaries [have been hired to lead key federal departments](https://www.gsa.gov/about-us/newsroom/news-releases/senate-confirms-robin-carnahan-to-lead-gsa-06232021). It’s an exciting time.

{{< tweet user="EmilieSimons46" id="1470392108339146756" >}}

What would it take for this to happen in Canada? It’s not super clear. The US had the failure of healthcare.gov [as its catalyzing moment for public sector tech](https://www.wired.com/2014/06/healthcare-gov-revamp/), the moment that made political leaders start caring about technology as a thing that could make or break their most important priorities. In Canada we had [Phoenix](https://en.wikipedia.org/wiki/Phoenix_pay_system) and …nothing substantially changed. 

(Or, more specifically – the Government of Canada _has_ invested substantially more money into IT projects over the past few years, but [without making any really fundamental changes](https://cds-snc.github.io/policy-politique/en/2019/delivering-services-differently/) to _how_ those IT projects are undertaken. That’s a problem.)


## To sum up

In Canada, we have a public service executive class that isn’t equipped to lead technology initiatives. We’ve got widespread adoption of digital government _words_, which has largely just made it harder to tell effective and ineffective implementation apart. And we’ve got a political class that is (understandably, these days) too busy with other things to care about the public service’s tech capacity. 

Not to mention: an [overdependence on contractors and consultants](https://www.tvo.org/article/consulting-firms-are-the-shadow-public-service-managing-our-covid-19-response), a [shortage of in-house digital expertise](/2020/05/26/why-are-there-so-few-senior-developers-in-government/), and a [lack of modern tools and equipment](/2020/12/27/tools-that-work/) for public servants.

Until something substantial changes – or a Phoenix-level crisis hits a public-facing service – we’ll all keep spending our time on [performative IT paperwork](https://federal-field-notes.ca/articles/2021-12-15-paperweight/) instead of building better services. 

<p><em>Was this post too bleak? Not bleak enough? Are you working in <a href="https://twitter.com/scott_pm/status/1445606630935040009" target="_blank">a pocket of government</a> that is doing awesome work? As always I’d <a href="https://twitter.com/sboots" target="_blank">love to hear your thoughts</a>!</em></p>
