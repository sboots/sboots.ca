---
title: "If you use project gating, you’re not agile"
subtitle: "It’s probably not your fault, though."
date: 2022-08-24T7:30:43-07:00
summary: "Short feedback loops are the secret to good software (and good IT projects), and years-long, pre-planned waterfall approaches are a fundamental barrier to achieving them. In the Canadian government, “project gating” is the main form this takes, where departmental teams seek approval (one gate at a time) to initiate a project, to get funding, to outline a project plan, an implementation plan, and a variety of other steps that eventually lead to building or procuring an IT system. Project gating is a relic from 25 years ago, and it’s past time for us to leave it behind."
extradisclaimer: "The views expressed here are my own, and don’t represent the opinions of my team or my employer."
images: ["/img/2022/whitehorse-obstruction-sign-2022.jpg"]
featured: true
---

There’s been a lot of interest in [adopting agile practices](https://www.canada.ca/en/government/system/digital-government/government-canada-digital-standards.html) in the Canadian government over the past few years. Being more incremental, iterating more quickly, and [breaking projects into smaller pieces](/2022/08/09/shrink-projects-to-fit-leadership-turnover-rates/) are all really valuable approaches. 

One of the major challenges facing digital teams in government is that – even if they organize their own work according to [agile principles](/2020/01/28/introducing-agile-to-large-organizations-is-a-subtractive-process-not-an-additive-one/) – they’re operating within a broader environment with a lot of constraints all built on waterfall thinking. “Waterfall” project management operates on the assumption that each step in building a thing or implementing a project can be done linearly, with all the planning done at the beginning and all the implementing done at the end.

Construction and engineering projects (building a bridge, for example) are the classic examples of waterfall project management. You know exactly what river you’re trying to cross, how much traffic the bridge will have to handle, and based on that you can plan out exactly what materials, people, and equipment you need, and build it according to those pre-planned specifications. ([Don’t do this](https://www.cbc.ca/news/canada/saskatchewan/bridge-that-collapsed-six-hours-after-opening-was-built-without-geotech-investigation-of-riverbed-reeve-1.4829890).)

Software development – including any government IT projects – doesn’t work like this (much as waterfall project managers would like to think that it does). Any software [that actually works](/2020/02/25/our-services-arent-working/#two-questions-that-are-actually-the-same-question) needs to account for the unpredictability of human behaviour. Doing that well involves repeatedly getting feedback [from the actual people that will use your software](https://federal-field-notes.ca/articles/2022-07-20-hire-a-designer-and-a-product-manager/#wont-somebody-think-of-the-users), and using that to continually improve what you’re building. [Short feedback loops](https://twitter.com/cooperlk99/status/1075737041734959104) are the secret to good software (and good IT projects), and years-long, pre-planned waterfall approaches are a fundamental barrier to achieving them.


## Documentation off-ramps, not implementation off-ramps

In the Canadian government, the main pressure to follow waterfall project management styles ([largely abandoned](https://tcf.pages.tcnj.edu/files/2013/12/ganis-tcf2010.pdf) by software companies outside government) originates [from financial management policies](https://www.tbs-sct.canada.ca/pol/doc-eng.aspx?id=32594), rather than information technology policies. 

**“Project gating”** is the main form this takes, where – in [a series of detailed planning steps](https://www.canada.ca/en/treasury-board-secretariat/services/information-technology-project-management/project-management/guide-project-gating.html) – departmental teams seek approval (one gate at a time) to initiate a project, to get funding, to outline a project plan, an implementation plan, and a variety of other steps that eventually lead to building or procuring an IT system. Project gating requirements might be enforced by a department’s CFO office, their CIO office, a major projects management office, or [some combination](/2022/08/09/shrink-projects-to-fit-leadership-turnover-rates/#smaller-and-better) of all three.

<figure>
  <img src="/img/2022/tbs-project-gating-fig2.jpg" class="img-fluid" alt="A flowchart titled “Key Decisions” with five boxes labelled from 0 to 5, with “Benefits realization” on the right after box 5. Each box includes a step such as “Verify business problem or opportunity”, “Validate business justification and select short list of options”, “Approve preferred option and approach”, and so on. Below the boxes is a set of flowchart icons indicating “go/no-go” decisions. Below that, in turn, is a set of boxes with “Preparation” steps, listing additional activities that are required for each step, such as “Articulate desired future state”, “Identify long list of options”, “Develop project management plan”, “Ensure capability is fit for purpose”, and so on.">
  <figcaption><span class="sr-only">Caption: </span>From the <a href="https://www.canada.ca/en/treasury-board-secretariat/services/information-technology-project-management/project-management/guide-project-gating.html#toc5">“Guide to Project Gating”</a>. Implementation – actually building or procuring a system – isn’t explicitly listed but it’s somewhere between step 4 and 5.</figcaption>
</figure>

The goals of project gating are ultimately [to provide off-ramps](https://www.canada.ca/en/treasury-board-secretariat/services/information-technology-project-management/project-management/guide-project-gating.html#toc2) where, for example, a poorly-defined or unnecessary project could be halted before it wastes more money. This is a worthwhile goal, and comparable in some ways to [what I wrote about a couple weeks ago](/2022/08/09/shrink-projects-to-fit-leadership-turnover-rates/) – splitting large projects into smaller ones that leaders feel more accountable for. 

The critical difference, however, is that **all of the project gating off-ramps take place in the planning stage**, not the implementation stage. The careful, excruciating scrutiny that takes place at each gate – accompanied by [hundreds of pages of documentation](https://federal-field-notes.ca/articles/2021-12-15-paperweight/) – all happen before any software is shipped, before any actual user sees it, and before any feedback or user research can come back in and improve what’s being built. 

Teams going through the project gating process are challenged on the quality and comprehensiveness of their upfront planning documentation, which (in general) is not only a waste of teams’ time, it has a downstream effect of extensively solidifying or “baking” decisions into that documentation in a way that _prevents_ the future iteration and responsiveness to feedback that’s required to build good software. 

Project gating is designed to prevent expensive IT project failures, but it’s worth keeping in mind that all of the Canadian government’s most notable IT failures in the past decade successfully completed a project gating process. You [may have heard of](https://www.federalretirees.ca/en/news-views/news-listing/may/auditor-general-report-on-phoenix-pay-system-an-incomprehensible) some of them.


## The long way back

I was curious about the origins of project gating in the Canadian government, beyond [the documentation that’s currently published on Canada.ca](https://www.canada.ca/en/treasury-board-secretariat/services/information-technology-project-management/project-management/guide-project-gating.html) (last updated in 2021). The Internet Archive’s [Wayback Machine](https://web.archive.org/) is a fantastic resource for this. 

The earliest reference I’ve seen to project gating is a 1997 TBS proposal for an [“Enhanced Framework for the Management of Information Technology Projects”](https://web.archive.org/web/20060628094221/http://www.tbs-sct.gc.ca/pubs_pol/ciopubs/tb_it/efm1_e.asp). It’s …not bad!

> Gating also allows the department to control the cost of projects and minimize the financial loss on problem projects. In this approach, a designated senior departmental official, e.g., the project sponsor, manages the funds allocated to the project and releases only the funds needed to reach the next gate to the project leader. The performance of the project is reviewed at each gate, or when the released funds run out (to avoid delays, the designated official could release sufficient funds to permit work to continue on the project for a short time while this review and decision took place). After the review, departmental management can decide to proceed with the project as planned, modify the project and/or its funding, or even terminate the project limiting the loss to the amount previously allocated.
> 
> Projects and contracts will have to be structured to avoid incurring major penalties from the application of gating. By requiring the contractor to provide complete information on project performance and progress and also specifying in the contract when the scheduled reviews are to take place, the reviews could be conducted in a reasonable time without the need to stop work. By specifying the option to cancel the contract at the scheduled gates including the criteria on which such a decision would be made, in the contract, gating can be implemented without incurring major penalties.

Even from the outset – 25 years ago! – it’s noteworthy that TBS acknowledged the potential burden that project gating could incur. As written, this feels [even more closely-aligned](/2022/08/09/shrink-projects-to-fit-leadership-turnover-rates/) with the goal of breaking large projects into smaller components. (It presupposes, however, that work [won’t be done in-house](https://www.belfercenter.org/publication/government-technology-silver-bullet-hiring-house-technical-talent), which is both disappointing [and prescient](https://pipsc.ca/news-issues/outsourcing/part-one-real-cost-outsourcing).)

Over the decades since, this idea transmuted into a more formalized set of gates, with increasingly-burdensome documentation requirements at each gate. This [2010 TBS document](https://tc.canada.ca/sites/default/files/migrated/irp_gpgitep_eng.pdf) provides a detailed overview of what had by then become the “seven-gate model”. Departments, in turn, developed their own variations and frameworks based on the TBS guidance at the time, in some cases requiring teams to complete several competing project management frameworks simultaneously for the same project.

{{% figurecaption src="/img/2022/whitehorse-obstruction-sign-2022.jpg" alt="A bright orange construction sign on the edge of a downtown Whitehorse street, saying “Obstruction Ahead” in capital letters." caption="Caution, metaphors." %}}

## There is no waterfall-agile combo; it’s just waterfall

A lot has been written on the downsides of combining waterfall and agile approaches. Nevertheless this is probably the most common project management style seen in government today, as teams (like [Honey’s](https://twitter.com/honeygolightly/status/1561679721846476801)) try to be as agile as they can within a broader financial and project management policy landscape that requires waterfall steps and documentation.

Here’s how [Mike Bracken](https://public.digital/people/mike-bracken), the original director of the UK’s Government Digital Service, [describes it](https://gds.blog.gov.uk/2015/07/10/you-cant-be-half-agile/):

> Being agile doesn’t mean you give up on governance or deadlines. The idea that agile somehow “needs” a waterfall-type methodology to give it **control and governance** is nonsense. When you work in an agile way, **governance is built into every step** of what you do. You build and iterate based on ongoing user research. You build what users need, not what you guessed might be a good idea before you even started building. That means spending money throughout the lifecycle of a service. Not throwing a lot of money at a project upfront, without knowing if it’s going to be useful. Or not.
> 
> In my view, formalising a mishmash approach is going to end up giving you the **worst of both worlds**. You won’t get the thing you planned on the date you planned it, and you won’t get something that meets user needs either. You’ll end up with something that fails on both counts.

[Paul Craig](https://twitter.com/pcraig3) has [an excellent post that speaks directly](https://federal-field-notes.ca/articles/2022-03-22-move-fast-stay-safe/#working-with-wagile) to the tension between shipping quickly – a key agile practice – and concerns around governance and oversight:

> Is ‘Wagile’ a good idea? [No](https://www.pluralsight.com/blog/it-ops/move-away-from-wagile). But how about starting fights with a bunch of people you work with and eventually having your project cancelled? Well, obviously that’s worse.
> 
> [It’s not easy to subtract governance processes](/2020/01/28/introducing-agile-to-large-organizations-is-a-subtractive-process-not-an-additive-one/) in an organization hyper-sensitive to risk (“let’s **not do** this documentation and still be allowed to release”). Removing something that _looks_ safe (even a diagram that will soon be out of date) without an equivalent replacement is a tough sell.
> 
> [Shipping early](/2020/01/10/shipping/) is the best argument you can make against the reality of waterfall, because, done right, you will save huge amounts of time and money. By the same token, the longer it takes you to get products built and released, the more you resemble the expensive waterfall processes you seek to replace.
> 
> This is why you _need_ to **move fast**. In general, you want to define your MVP and then test it with users as soon as possible. Enterprise planning does not have a good answer to ‘user needs’, so it is important to prioritize early user engagement. User feedback both (a) gives you insight to improve your product and (b) functions as documentation you can share internally that other teams don’t typically have. Once you are confident that your product works, focus on what you need to do to get it released. It’s far better to have a released ‘alpha’ service than a highly-polished internal prototype.

[Ashley Evans](https://twitter.com/ashlevanss), [Sarah Ingle](https://www.linkedin.com/in/sarahlmingle/) and [Jane Lu](https://www.linkedin.com/in/janelu1/) wrote a really fantastic post on a similar theme, on [what it looks like to shift from planning to learning](https://medium.com/good-trouble/shifting-from-planning-to-learning-74e217561f65). They write:

> The root problem is a desire to avoid failure by overplanning and creating a sense of false certainty.
> 
> From a structural perspective, this barrier shows up as excessive forms to fill out, briefings to give, or checklists to complete.
> 
> From a cultural or behavioural perspective, it shows up as top-down decision-making, discouragement of change, or critique without support to find an alternative.
> 
> We need to redesign go-live protocols and digital governance processes so that they are contextual, and encourage creativity, responsible design, and learning over compliance, oversight, and risk-avoidance.

Canada isn’t alone in having departmental funding models that reinforce outdated ways of working; written from the UK, [Emma Stace](https://twitter.com/Emmastace)’s excellent [list of top issues facing government in implementing digital, data, and technology strategies](https://medium.com/@emmastace/top-issues-facing-govt-in-implementing-digital-data-and-technology-strategies-2848ad381f42) captures this well:

> Funding can be a root cause of poor technology. Technology funded as a capital investment or project with a start and finish date not only locks in legacy thinking about tech as a ‘cost centre’, it also increases cost, duplication and fragmentation by effectively starting from ‘0’ every time.
> 
> Change the way your organisation funds technology by determining its value, not its cost.


## Waterfall opt-out strategies

For teams in government that want to be agile – hopefully that includes you! – one way to navigate these constraints is _to not structure your work as projects_, since formal project gating requirements originate in government-wide project management policies. [Remy Bernard](https://twitter.com/remyb2) from ESDC’s IT Strategy team has [a really interesting post](https://sara-sabr.github.io/ITStrategy/2022/07/21/funding-sw-activities.html) that looks at this in more detail.

Projects by definition have a defined start and end date; most government services don’t “stop” at a specific point in the future. Structuring improvements to existing services (or the development of a new service) into a time-bound “project” is another waterfall side-effect that leads to [semi-abandoned, legacy systems that still power critical public services](https://medium.com/the-technical-archaeologist/old-code-gets-younger-every-year-3bd24c7f2262) but that don’t have an ongoing team or funding available to keep improving them. Projects are “done”, but software that’s actively being used by human beings [never is](https://twitter.com/arvidkahl/status/1539781563923193857).

In departments that have funding already available, teams might be able to describe their work – accurately – as an “initiative” or as a service, which is a better articulation of responsible stewardship of critical systems than a time-limited project would be. Some departments’ financial approval processes consider any initiative larger than $2 or $3 million a project “automatically”, making this strategy less feasible. If nothing else, that’s extra motivation to keep your IT initiatives [small and incremental](/2022/08/09/shrink-projects-to-fit-leadership-turnover-rates/).

For departments that are seeking new funding, the strategy I’d strongly recommend is to seek [funding for teams, not projects](https://defradigital.blog.gov.uk/2017/09/19/lets-fund-teams-not-projects/). This avoids baking untested assumptions into project plans and funding proposals. The team, once it forms, is [better equipped](https://federal-field-notes.ca/articles/2022-07-20-hire-a-designer-and-a-product-manager/) to iterate, gather feedback, and change approach based on what they learn. And, ideally, they can continue incrementally improving their IT systems and services well into the future, beyond the constraints of a project end date. 

One of the critiques of agile software development that frequently comes up is that “it’s workable for smaller, experimental projects, but it doesn’t work well for really big projects”. The truth (as one of [Paul](https://twitter.com/pcraig3)’s colleagues at [GDS](https://gds.blog.gov.uk/) once said) is that _no one_ has a process that works well for larger projects. Larger projects [just tend to go wrong](https://large-government-of-canada-it-projects.github.io/#are-large-it-projects-likely-to-be-successful), whether you use agile or [SAFe](https://twitter.com/allenholub/status/1544383452522299392) or PRINCE2 or any other project management approach. You just [shouldn’t do mega-projects](/2022/08/09/shrink-projects-to-fit-leadership-turnover-rates/).

I’d love to see the project gating framework and related policy requirements be formally deprecated in the future; it’s a decades-old relic that has more downsides than benefits. [Getting rid of project gating](/2020/01/28/introducing-agile-to-large-organizations-is-a-subtractive-process-not-an-additive-one/) is asking a lot of senior public service leaders – to do things smaller and more incrementally, to trust their teams, and to [relinquish a degree of control](https://twitter.com/Code4Luke/status/1560353078330773506) (especially if they’re in an oversight or gatekeeping role that’s outside a team’s own reporting hierarchy). But the longer we keep it, the longer we’ll be stuck in a non-agile past.

{{< tweet user="allenholub" id="1559587771714502660" >}}

_Interested in learning more? [Unit 3 on Iteration](https://www.notion.so/Unit-3-Iteration-935dbdea1dd44eb59caf69fa0a263b67) of the [Teaching Public Service in the Digital Age](https://www.teachingpublicservice.digital/) publicly-available syllabus is a great, in-depth read. This [Beeck Center](https://beeckcenter.georgetown.edu/) case study – [Lessons from the Digital Transformation of the UK’s Universal Credit Programme](https://beeckcenter.georgetown.edu/lessons-uk-universal-credit/) – is also a fantastic summary of what doing this work well looks like._
