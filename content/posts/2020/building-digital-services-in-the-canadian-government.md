---
title: "A short introduction to building digital services in the Canadian government"
slug: "building-digital-services-in-the-canadian-government"
date: 2020-06-16T16:30:31-07:00
summary: "Building digital services and IT systems in a government environment is complicated. The federal government in particular has a lot of rules to navigate, and it’s easy for these to overwhelm people and siphon their time away from designing and building user-friendly software. This short guide was written for an audience that’s used to building digital products in the private sector, to better understand what’s new and different in a government context. Enjoy!"
extradisclaimer: "This was written on a weekend for friends in the civic tech community. This isn’t formal Government of Canada policy advice."
images: ["/img/2020/parliament-feb-2020.jpg"]
featured: true
---

Back in March, some friends from the Ottawa civic tech community reached out. The pandemic was [ramping up](/2020/03/25/look-out-for-one-another/), and they were interested in volunteering their developer skills to help government departments respond to the crisis. Building digital services and IT systems in a government environment is complicated. The federal government in particular has a lot of rules to navigate, and it’s easy for these to overwhelm people and (at the least) siphon their time away from designing and building user-friendly software.

Here’s what I wrote, on a Sunday evening – none of this constitutes formal policy advice, but it was meant to give an introduction to which rules really do deserve a lot of attention, and potential landmines to avoid. (Note that some of the links below were added to this blog post after the fact, for extra context or further reading.) 

You’ll notice that this skips over some of the most important practical steps in designing, delivering, and iterating on good digital services – doing research with actual users, using [modern software development tools](https://digital.canada.ca/2018/06/27/tools-to-do-good-work/) and best practices, deploying early and frequently, etc. This was written for an audience that’s used to building digital products in the private sector, to better understand what’s new and different in a government context. Enjoy!

<img src="/img/2020/parliament-feb-2020-cropped.jpg" class="img-fluid" alt="A photo from near Parliament Hill looking west at the Confederation Building and other buildings along Wellington, on a sunny February day.">

## A short introduction

In case it’s useful, here’s a few suggestions on typical government implementation details – trying to focus here on the ones that really matter, not the seemingly-endless lists of rules that [ultimately don’t affect users](/2020/02/27/user-needs-not-government-needs/). These are the ones that government teams get accidentally crushed over when they screw them up (e.g. lawsuits or public shaming, etc.). 

From a tech standpoint, anything you build is [almost guaranteed](/2020/05/26/why-are-there-so-few-senior-developers-in-government/) to be higher-quality than most existing GC systems and services. Use what you’re familiar with and what you trust. Most of these suggestions ultimately have to do with the front-end/public-facing aspect of services, not back-end engineering decisions (where the GC norm is, y’know, [40-year-old COBOL](https://www.macleans.ca/politics/ottawa/pulling-off-a-bureaucratic-miracle-how-the-cerb-got-done/) or dicey ASP.NET applications).

_GC = Government of Canada; sorry in advance for any acronyms_

## Official Languages

Anything that constitutes a Government of Canada service or communications product needs to be available in English and French, “[simultaneously and of equal quality](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=26164)”. Ideally your departmental partner would have translation capabilities on standby so you wouldn’t need to translate things yourself – but you definitely need to build EN/FR internationalization support into everything from the start. Speaking from experience it’s a pain to add in after the fact. Publicly launching a service only in English, then adding French later, would be a huge (political) catastrophe.

Also count on at least one full business day for any translation request to come back, even ones that are marked super urgent. Write as much of your public-facing content as early as possible (e.g. in parallel to your software work) so that you can send it translation ASAP.

## Accessibility

Any Government of Canada service (and ones delivered and built by third parties) needs to meet **[WCAG 2.0 AA](https://www.w3.org/TR/WCAG20/)** accessibility standards. This is mostly the basics e.g. keyboard navigable, has sufficient colour contrast, has good headings and image alt-text, etc. 

Not meeting WCAG 2.0 AA is a semi-frequent source of lawsuits that the Government of Canada always loses. Run your service through at least two or three different online testing tools that check for WCAG compliance and save a copy of the results somewhere, send them to your departmental partners for posterity, etc. Your departmental partner should be doing much more extensive, ongoing accessibility testing (the [CDS accessibility handbook](https://digital.canada.ca/a11y/) can help).

## Federal Identity Program

Certain government types are _very_ particular about how the government’s logos and visuals are used. The very short answer is: put the [“Government of Canada / Gouvernement du Canada” signature](https://raw.githubusercontent.com/cds-snc/node-starter-app/master/public/img/sig-blk-en.svg) in the top left of the page, and the [“Canada” wordmark](https://raw.githubusercontent.com/cds-snc/node-starter-app/master/public/img/wmms-blk.svg) in the bottom right, and don’t be too outlandish with fonts and colours. (The formal [Federal Identity Program requirements](https://www.canada.ca/en/treasury-board-secretariat/services/government-communications/federal-identity-program/manual.html) are from the 1990s and mostly apply to government letterhead, building signs, and vehicle decals – there’s a lot of interpretation and debate about how to apply them to websites, and it’s best to avoid those debates if you can.) 

On the French version of your website or service, the signature should use the [French-first “Gouvernement du Canada / Government of Canada” version](https://raw.githubusercontent.com/cds-snc/node-starter-app/master/public/img/sig-blk-fr.svg).

CDS has [a “starter app” repository](https://github.com/cds-snc/node-starter-app) that you can use for inspiration (and logo files) but don’t worry too much if you’re using a different front-end library, etc.

## Domain names

The government is pretty inconsistent here, but in a perfect world everything run by the GC would have domain names ending in `*.canada.ca` or `*.gc.ca`. 

When Global Affairs Canada sent out notifications to a bunch of international travellers last week [mid-March] and used bitly links, people freaked out because [it looked like a scam](https://twitter.com/xdr/status/1240710656841486336).

There’s a [DNS setup](https://alpha.canada.ca/en/instructions.html) that CDS operates at `alpha.canada.ca` and can spin up a subdomain off of it relatively quickly, if that’s useful (and if your departmental partner doesn’t already have some specific URL in mind). It can be pointed at whatever cloud provider you need and it’s faster than going through the gauntlet of SSC + TBS + ServiceCanada that normally has to approve GC subdomains. It’d be better than something that isn’t clearly GC-operated. 

## Inclusive design

Practically speaking, this is probably the hardest area to figure out (but [incredibly important](/2020/02/25/our-services-arent-working/#why-this-matters)). Think about situations like: people applying for a service on behalf of their elderly non-tech-savvy parents; band councils trying to apply on behalf of everyone on their First Nations reserve; people applying on behalf of hospitalized family members or friends. 

One notable mishap here last year was IRCC’s redesigned program to apply for family reunification visas; the team built a cloud service (for the first time) and it scaled really well to handle the giant surge of requests when the application period opened (compared to, well, IRCC’s normal, more fragile IT systems). But, the program was designed “first come, first serve” and as a result, [inadvertently prioritized whoever could get through the complicated online application form fastest](https://www.cbc.ca/news/politics/ircc-parent-grandparent-sponsorship-filled-2019-1.4995806) (disadvantaging people with disabilities or accessibility requirements, people with slow bandwidth or computers, etc.).

People acting on behalf of other people is the most complicated area (and a bunch of GC services don’t handle it well, although the CRA and ESDC do have some online services that include delegating to family members / power of attorney contacts or, say, tax professionals). Whatever you build might not need to handle these edge cases, but figuring out ahead of time which ones you can and which ones you can’t (and clearly documenting why, and making sure that your departmental partners know) is important.

## Shipping

In government, the hardest part of any IT-related project is [literally getting it out the door](/2020/01/10/shipping/). Under normal circumstances there’s a whole gauntlet of approval processes (security, privacy, quality control, infrastructure) usually all done by separate groups or committees. For a brand new online service, getting through these processes could typically take 6-24 months. (This is one reason why people say that tech implementation is only a small part of digital government work – the rest is, either [navigating through or getting rid of all these waterfall processes](/2020/01/28/introducing-agile-to-large-organizations-is-a-subtractive-process-not-an-additive-one/)).

In an emergency situation like the COVID pandemic, the typical approval processes for something to get shipped (“go live” or “go into production”) could potentially be skipped – but in place of them, you would definitely need some kind of written confirmation from a senior public servant (e.g. assistant deputy minister or deputy minister) from the department in question. An email from them saying “I authorize the operation of this service” is sufficient. 

**There is a whole graveyard littered with amazing digital products in government that never made it out the door.** I can think of probably a dozen examples. Don’t be one of them. World-class tech implementation won’t get you through this; you need the backing from a public servant at the highest leadership level possible to fight through any potential gatekeepers and to give the green light to go live. Having a close relationship between the product team and that senior public servant from as early on as possible helps (direct communications, regular progress updates). I’d say, this is the biggest risk to any project – that you build something phenomenal, and then your partner department gets cold feet and it never ships. This happens frequently.

_Thanks to [Ross Ferguson](https://twitter.com/rossferg) for suggesting that I publish this as a blog post. If you’re a public servant working to navigate these rules in your department, [don’t hesitate to reach out](https://twitter.com/sboots)! The rules here – and the long tail of other government requirements – can definitely be a challenge, and you’re not alone._
