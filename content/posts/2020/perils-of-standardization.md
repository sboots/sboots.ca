---
title: "Perils of standardization"
date: 2020-02-04T21:34:46-05:00
subtitle: "“We only use Oracle databases from 2004. They’re a good vintage.”"
summary: "If you work in government IT, you’ve probably heard this before: “We’ve got one standard database product.” “We’ve standardized on this programming language.” “This software is our standard for case management systems,” and so on. There are a number of important downsides, though, to standardization efforts: one size all ends up fitting nothing well, they act as a placeholder for more informed technical discussions, and they end up being a barrier to continual change."
images: []
---

If you work in government IT, you’ve probably heard this before. “We’ve got one standard database product.” “We’ve standardized on this programming language.” “This software is our standard for case management systems,” and so on.

This isn’t unique to government, and it isn’t intrinsically a bad thing. Some standards are incredibly valuable; for example, there’s [only one right way to write date formats](https://en.wikipedia.org/wiki/ISO_8601#Calendar_dates). Software standards that improve a user’s experience (for example, using single sign-on instead of having dozens of separate login accounts) are a great choice. 

But, standardization often plays an outsized role in technology strategy or enterprise architecture. Standardizing (or consolidating) on a single set of systems, or on a single product for a specific use-case, or on a single vendor, becomes [a goal in itself](https://www.ribbonfarm.com/2010/07/26/a-big-little-idea-called-legibility/) – often without recognizing the tradeoffs that end up being made as a result. In this blog’s spirit of being [gently counter-cultural](/2020/01/21/principles-for-blogging-as-a-public-servant/#how-to-criticize-a-thing-that-you-love), here are some downsides to standardization efforts.

## One size all fits nothing well

In conversations about enterprise software (that is, software marketed at large organizations like multinational companies, universities, and government institutions), poor usability comes up pretty frequently. These are software products that are expensive, incredibly complex, do a lot of things, and are somehow almost always very, very difficult to use. There’s [a great Twitter thread from Arvind Narayanan about Blackboard](https://twitter.com/random_walker/status/1182635589604171776), an enterprise courseware product used by a lot of universities and colleges. Arvind writes,

> [Blackboard is] actually designed to look extremely attractive to the administrators (not professors and definitely not students) who make purchase decisions. Since they can't easily test usability, they instead make comparisons based on… checklists of features. 🤦🏽‍♂️
> 
> And that's exactly what's wrong with Blackboard. It has every feature ever dreamed up. But like anything designed by a committee, the interface is incoherent and any task requires at least fifteen clicks (and that's if you even remember the correct sequence the first time).

There’s a lot of reasons why “everything and the kitchen sink” is a common philosophy for enterprise software, especially when it’s sold to governments. Government procurement is difficult and time-consuming, so buying one product that does “everything” (instead of several separate products) is appealing. Checklists of features, as Arvind describes, are easier to communicate through [RFP](https://en.wikipedia.org/wiki/Request_for_proposal) responses (in long paper documents) than the usability or intuitiveness of a software’s interface, or how happy or frustrated people are when they use it. And, complicated review processes for security and privacy mean that it’s easier to just use one product for as long as possible.

The downside is that – as a result – these “one size fits all” enterprise software products are hard for people to navigate and use, which makes people’s work more frustrating and less efficient. These products often also need to be extensively customized in order to work for the organization buying them, which can be time-consuming and introduce unexpected and hard-to-detect software bugs.

## A placeholder for more informed technical discussions

Over time, it’s easy for standardization – as a goal in itself – to replace more informed discussions about the merits and downsides of different technology options. In environments where there is limited technical expertise (a frequent issue in government institutions), standardization is a simple enough concept that it can become a stand-in for actual technical discussions. Making the case for a particular technology tool or framework instead of another can quickly reach a level of complexity that decision-makers aren’t comfortable with. Asking “is it standard?” gives the appearance of a technical discussion without actually providing it.

In situations like this, the best approach is to [learn to ask better questions](https://github.com/18F/technology-budgeting/blob/master/handbook.md#appendix-a-questions-to-ask). Does using one technology instead of a different one speed up people’s work, or slow them down? Does it make a service more accessible? Does it make it easier, or harder, to reliably get data in and out of a system? These are all more important questions – when it comes to the outcomes that a technology decision should achieve – than “is this technology the standard”.

## A barrier to continual change

Governments and institutions that decide on widely-held standardized software products aren’t able to easily change these when the products get out of date. Standardized technology decisions can [remain in place for many years](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=25687), even as the technology industry moves past them. Even if the decisions were thoughtfully made at the time, they almost always remain in place long past the point where they add value. **Standards end up staying in place much longer than they should, because removing or changing them takes more political capital than anyone is willing to spend.** Even if the most cutting-edge technologies were selected – for a standard database product, standard programming language, standard case management system, or standard software for any other purpose – it’s just a matter of time until they’re a detriment instead of a benefit.

Over time, as these standards get more and more out of date, they add increasingly severe side effects: preventing teams from being to experiment with new technology choices, introducing security vulnerabilities as products get end-of-lifed by manufacturers, and discouraging expert talent from wanting to work for your institution. If you only use really old database products – or, for that matter, if you only build things in Java or ASP.NET – you’re not going to be able to hire the talented software developers and technology experts you need.

No standard can keep up with the pace of change in technology, especially in the web development world. The main takeaway for government institutions is: don’t mandate specific systems. As [Marianne Bellotti writes](https://medium.com/@bellmar/sre-as-a-lifestyle-choice-de9f5a82d73d),

> No matter how thoughtfully written or well researched a policy is someone, somewhere in government will create failure from enforcing it. It is inevitable. 

The plot twist is: **standards can be a force for good, when they equip organizations to be better able to keep pace with change instead of slowing them down**. The UK’s [Digital Service Standard](https://webarchive.nationalarchives.gov.uk/20161210205948/https://www.gov.uk/service-manual/service-standard) and [Technology Code of Practice](https://webarchive.nationalarchives.gov.uk/20170909132908/https://www.gov.uk/government/publications/technology-code-of-practice/technology-code-of-practice) did this really well, by introducing open source requirements and shorter maximum lengths for IT contracts. Standards that keep your options open and avoid vendor lock-in can be tremendously valuable.

Instead of mandating specific software products and systems, mandate [ways of working that lead to good outcomes](/2020/01/10/shipping/#how-to-make-shipping-easier). When it comes to software choices, government institutions should mandate interoperability, full data import and export capabilities, and other approaches that keep their future options open.

_Like this? Read Dan Sheldon’s [Government IT Self-Harm Playbook](https://medium.com/@sheldonline/the-government-it-self-harm-playbook-6537d3920f65#9156) from 2016._
