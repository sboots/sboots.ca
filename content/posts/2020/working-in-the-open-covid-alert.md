---
title: "“Working in the open” firsts for COVID Alert"
date: 2020-10-30T15:27:32-07:00
summary: "Working on COVID Alert has definitely been a career highlight, in a lot of unexpected ways. As of this week more than 4.8 million people have downloaded the app, and 2,600 people have used it to alert people close to them about their COVID exposure. For everyone that has worked on COVID Alert, it’s humbling and daunting to be part of something at this scale. COVID Alert also included some extra geeky “firsts” in the Canadian government that I was really thrilled to see, all related to working in the open."
subtitle: "Make things open, it makes things better."
images: ["/img/2020/covid-alert-iphone.jpg"]
---

A few months ago I wrote about [how busy the summer ended up being](/2020/07/29/a-busy-couple-months/). Working on [COVID Alert](https://www.canada.ca/en/public-health/services/diseases/coronavirus-disease-covid-19/covid-alert.html) has definitely been a career highlight, in a lot of unexpected ways in an unexpected year. As of this week [more than 4.9 million people](https://www.canada.ca/en/public-health/services/diseases/coronavirus-disease-covid-19/covid-alert.html#a5.5) have downloaded the app, and 2,900 people have used it to alert people close to them about their COVID exposure. For everyone that has worked on COVID Alert, it’s humbling and daunting to be part of something at this scale. 

<img src="/img/2020/covid-alert-iphone-cropped.jpg" class="img-fluid" alt="An iPhone on a wood-panel desk, showing the COVID Alert app with a message that says “No exposure detected”.">

In a lot of ways, COVID Alert represents some unprecedented milestones in Canadian federal government IT: 

* It’s the first large-scale, public-facing mobile app launched by the Government of Canada [that is open-source](https://github.com/cds-snc/covid-alert-app), to my knowledge. (A lot of that is credit to the volunteer team that built [COVID Shield](https://www.covidshield.app/), the proof-of-concept app that COVID Alert is based on!) 
* It was built [in 45 days](https://digital.canada.ca/2020/07/31/continuously-improving-covid-alert/), between the day that [CDS](https://digital.canada.ca/)’s product team was formed and the public launch of the app. 
* It had [a pre-launch public beta](https://twitter.com/CDS_GC/status/1285771764900012032) where thousands of people helped test the app and provided feedback. 
* And, it involved some very close collaboration between the federal government and provincial healthcare and technology teams [to deliver one-time keys to COVID-positive patients](https://digital.canada.ca/2020/09/03/meeting-the-needs-of-healthcare-authorities-to-roll-out-covid-alert-across-canada/).

Beyond all of that, there were some extra geeky “firsts” that I was really thrilled to see, as someone working at the intersection of tech and policy. Each of these are different (really neat) examples of [working in the open](https://www.gov.uk/guidance/government-design-principles#make-things-open-it-makes-things-better).

## A privacy assessment published in the open

Protecting Canadians’ privacy was one of the foremost goals of the entire project. If Canadians didn’t trust COVID Alert and didn’t adopt it in sufficient numbers, it wouldn’t have any public health impact. Ensuring users’ privacy was one of the main benefits of the underlying [Google/Apple exposure notification framework](https://covid19.apple.com/contacttracing), and building the app [as an open source project](/2020/08/20/make-things-open-source-it-makes-things-better/#when-public-trust-matters-most) gave privacy, security, and technology experts the ability to [dig into the code and point out any privacy concerns](https://seancoates.com/blogs/how-i-helped-fix-canadas-covid-alert-app).

One of the highlights of my day-to-day work on COVID Alert was working with Health Canada’s privacy division on the [COVID Alert Privacy Assessment](https://github.com/cds-snc/covid-alert-documentation/blob/main/COVIDAlertPrivacyAssessment.md) and the wide range of other privacy documentation that went into the design and oversight of the overall system. Health Canada’s privacy team is second to none. Their thoughtful feedback, questions, and deep understanding of Canada’s federal privacy environment made working on a complicated topic a really wonderful experience.

The privacy assessment was published both [on GitHub](https://github.com/cds-snc/covid-alert-documentation/blob/main/COVIDAlertPrivacyAssessment.md) and [on Canada.ca](https://www.canada.ca/en/public-health/services/diseases/coronavirus-disease-covid-19/covid-alert/privacy-policy/assessment.html) the day the app launched. As far as I know, it’s the only full privacy assessment for an app or online service that the federal government has ever proactively published. (If you know of any others, let me know!)

## A public Accessibility Statement

[Accessibility statements](https://www.w3.org/WAI/planning/statements/) are [an emerging best practice](https://www.gov.uk/guidance/make-your-website-or-app-accessible-and-publish-an-accessibility-statement#publish-your-accessibility-statement) for organizations and websites, where they detail how they’re meeting accessibility needs, what issues are still outstanding, and provide ways for people to provide feedback or raise issues. A number of European countries [now require accessibility statements](https://eur-lex.europa.eu/eli/dir/2016/2102/oj) on public sector websites.

[COVID Alert’s Accessibility Statement](https://www.canada.ca/en/public-health/services/diseases/coronavirus-disease-covid-19/covid-alert/accessibility-statement.html), published on Canada.ca, is the federal government’s first-ever accessibility statement for a mobile app. (It’s the second-ever published accessibility statement, after a [2018 accessibility statement for an ESDC consultation tool](https://esdc-consultations.canada.ca/accessibility) run by a third-party vendor). COVID Alert’s Accessibility Statement is accompanied by [an accessibility report, published on GitHub](https://github.com/cds-snc/covid-alert-documentation/blob/main/AccessibilityReport.md), that details ongoing issues and work in progress. 

My colleague [Julianna](https://twitter.com/JuliannaRowsell) – a fearless advocate both inside and outside CDS for accessibility and inclusive design – [championed both of these](https://twitter.com/JuliannaRowsell/status/1289231164767703041) in really thoughtful ways as COVID Alert came together.

## A Vulnerability Disclosure Policy for cybersecurity researchers

Last but not least! [Vulnerability disclosure policies](https://www.hackerone.com/blog/Vulnerability-Disclosure-Policy-Basics-5-Critical-Components) (VDPs) are quickly becoming a norm for both tech companies and government institutions. They let cybersecurity researchers know what things they can and can’t do while poking at websites or services to make sure they’re secure, and how to notify the organization’s security teams if they find something broken.

Vulnerability disclosure policies are an important signal to cybersecurity researchers that a team or organization takes cybersecurity seriously. That if they notice something broken or unsecured, that they can report it to the organization in an obvious way – without worrying that they’ll be accused of hacking or illegal activity when they’re trying to help. Both the [UK government](https://www.ncsc.gov.uk/blog-post/vulnerability-co-ordination-pilot) and the [US government](https://www.cisa.gov/blog/2020/09/02/improving-vulnerability-disclosure-together-officially)’s cybersecurity agencies have been making vulnerability disclosure policies into a standard process over the past few years.

[COVID Alert’s Vulnerability Disclosure Policy](https://github.com/cds-snc/covid-alert-documentation/blob/main/VulnerabilityDisclosurePolicy.md) is the first VDP ever published by the Government of Canada. There’s still work ongoing to make this a regular part of launching and operating government websites and services – I’m really excited to see where it goes.

## Onwards and upwards

I’m really grateful to have been able to work on COVID Alert, and in total awe of my software development, design research, design, and product management colleagues that [made it a reality](/2020/01/10/shipping/). Working with the talented team at Health Canada has also been a huge highlight. (And, not least, with [Sam](https://twitter.com/TheSamBurton) and [Lucas](https://twitter.com/lchski) and [Michael](https://twitter.com/supergovernance) and [John](https://twitter.com/JohnMillons) and the whole CDS policy team! Y’all are the very best.)

People’s [reactions](https://www.michaelgeist.ca/2020/10/four-million-downloads-and-counting-everyone-should-install-the-covid-alert-app/) [to](https://www.cbc.ca/news/canada/prince-edward-island/pei-app-federal-covid-aug-1-2020-1.5670768) [the](https://twitter.com/lhochstein/status/1294762688753446912) [app](https://www.linkedin.com/feed/update/urn:li:activity:6696905550967394304/) [have](https://twitter.com/cyberpolicyx/status/1289259262380609536) [been](https://twitter.com/PhilHoldsworth/status/1289236457488490498) [really](https://twitter.com/alox/status/1289240527330656256) [really](https://twitter.com/_RobertLowe/status/1286023811968770055) [positive](https://twitter.com/MRT1N_/status/1286108745165135873), and I hope we can maintain that level of public trust as the app continues to improve. If you want to learn more about how it came together, [check out the official CDS blog for an ongoing series of posts on how COVID Alert was built](https://digital.canada.ca/blog/).
