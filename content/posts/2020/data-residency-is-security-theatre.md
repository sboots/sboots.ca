---
title: "Data residency is security theatre"
date: 2020-03-29T22:11:28-07:00
summary: "One of the most persistent myths in Canadian government IT is that storing your data in Canada protects it against eavesdropping or interception by foreign governments. If someone on your government team has asked to use a new online tool and your reaction is, “no, you can’t, because it’s hosted in the United States,” this article is for you."
extradisclaimer: "The views expressed here are my own, and don’t represent the opinions of my team or my employer."
images: ["/img/2020/downtown-boston-2019.jpg"]
---

One of the most persistent myths in Canadian government IT is that storing your data in Canada protects it against eavesdropping or interception by foreign governments. Storing your information in data centres geographically located in Canada, the claim goes, or using cloud services that are fully hosted in Canada, safeguards you against your data being intercepted by, say, U.S. intelligence agencies.

If someone on your government team has asked to use a new online tool and your reaction is, “no, you can’t, because it’s hosted in the United States,” this article is for you.

For Canadian public servants, data residency concerns [mostly originate from the USA PATRIOT Act](https://www.tbs-sct.gc.ca/pubs_pol/gospubs/TBM_128/usapa/faq-eng.asp#Q1), introduced in 2001 following the 9/11 attacks. The PATRIOT Act gives U.S. law enforcement and intelligence agencies a broad ability to intercept and collect electronic information without informing the persons whose information is being gathered. Although the PATRIOT Act has been in place for almost twenty years, it wasn’t until a few years ago (as the Canadian government began to adopt cloud services) that formal data residency requirements were introduced.

## Consequences of data residency requirements

Canada’s adoption of cloud services comes several years behind most comparable governments. Around the world, governments and leading private sector companies have all adopted cloud services in earnest, for everything from front-line service delivery to internal collaboration tools. 

Cloud services (operated by third-party companies and accessed over the internet) are [updated and improved regularly, can be easily and reliably scaled, and typically cost much less](https://www.canada.ca/en/government/system/digital-government/modern-emerging-technologies/cloud-services/government-canada-cloud-adoption-strategy.html#toc2) than custom software hosted in traditional data centres. Using “software as a service” tools (where an online application and the infrastructure it runs on are both operated by a third-party company) has become an integral part of software development, collaboration, and team communication for [modern organizations](https://public.digital/2018/10/12/internet-era-ways-of-working/).

Canadian government departments have [nominally been able to use](https://twitter.com/Lance_Valcour/status/1075760866052714497) software-as-a-service tools with protected information since 2017. Government-wide policies [explicitly encourage the adoption of cloud services](https://www.canada.ca/en/government/system/digital-government/modern-emerging-technologies/cloud-services/government-canada-cloud-adoption-strategy.html#toc6-3), especially software-as-a-service products. However, data residency requirements applied to [Protected B information](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=32614) mean that most software-as-a-service tools – which are almost all hosted outside of Canada – can’t be used by government teams that need to handle this level of information. Moreover, widely held misconceptions that no Canadian government data can be stored outside of Canada have significantly hampered the adoption of cloud services.

Data residency requirements – and the myths that have accompanied them – have slowed the adoption of modern cloud services in government. In place of the professional-grade software used by other governments and companies, Canadian government teams end up depending on legacy IT systems. Or, they end up adopting mediocre imitations of widely-used software, where the selling feature is that the product is hosted in Canada rather than being user-friendly, reliable, scalable, or cost-effective.

Canada is too small a market for any but the largest cloud service providers to launch dedicated infrastructure here. Data residency requirements limit software options to major providers and exclude small software-as-a-service companies and products that are widely used elsewhere.

## Your data will be monitored anyway: a historical overview

Proponents of data residency requirements argue that, by storing government information in the United States, it will become subject to U.S. surveillance and infringe on people’s privacy rights as a result. But developments over the past two decades suggest that – no matter where information is stored – it’s subject to intelligence or law enforcement monitoring anyway.

### Boomerang routes

In the years following the introduction of the PATRIOT Act, a major concern was that Canadian internet traffic frequently crisscrosses U.S. borders, and would be intercepted and monitored when it crossed. Researchers at the University of Toronto and York University pointed out that most Canadian internet traffic – even when it starts and ends within Canada – is [routed through internet infrastructure in major U.S. cities](https://ixmaps.ca/) (so-called “boomerang routes”). 

Internet networking systems automatically optimize for the fastest and most reliable routes – that’s part of what makes the internet resilient – and the fastest networks between two points in Canada often travel through the United States. Although this doesn’t apply to dedicated (standalone) corporate networks, any Canadian citizen interacting with a government service online would be potentially subject to U.S. monitoring as a result.

### Edward Snowden and the reach of U.S. electronic monitoring

In 2013, former U.S. intelligence contractor Edward Snowden [revealed](https://www.theguardian.com/world/2013/dec/09/edward-snowden-voted-guardian-person-of-year-2013) that U.S. electronic surveillance [extends much further](https://www.theguardian.com/world/2013/nov/02/nsa-portrait-total-surveillance) than had previously been publicly known:

> a dragnet programme to scoop up digital activities direct from the servers of the biggest US tech companies; a tap on fibreoptic cables to gather huge amounts of data flowing in and out of the UK; a computer program to vacuum up phone records of millions of Americans; a codebreaking effort to crack the encryption system that underpins the safety and security of the internet.

Snowden’s revelations make it fairly clear that information stored anywhere in the world is potentially subject to U.S. intelligence monitoring. Ironically, the country where it’s likely the hardest for U.S. intelligence groups to monitor is the United States itself, since they would need to get [FISA court](https://en.wikipedia.org/wiki/United_States_Foreign_Intelligence_Surveillance_Court) or domestic law enforcement approval to potentially monitor American citizens:

{{< tweet 1000025567427776512 >}}

Foreign intelligence agencies running misinformation campaigns [reportedly use servers located in the United States](https://www.nytimes.com/2020/02/20/us/politics/russian-interference-trump-democrats.html) for this exact reason.

### The Microsoft Ireland court case

As part of an unrelated law enforcement investigation in 2013, a U.S. judge [issued a warrant](https://en.wikipedia.org/wiki/Microsoft_Corp._v._United_States) requiring Microsoft to produce emails and information associated with a user account allegedly related to drug trafficking. The emails were stored on Microsoft servers located in Dublin, Ireland, and Microsoft argued that a U.S. judge did not have the authority to issue warrants for information located outside the United States. 

In 2014, a federal judge declared that the legislation the warrant was based on (from 1986) acted as a subpoena and was [not restricted](https://harvardlawreview.org/2015/01/in-re-warrant-to-search-a-certain-email-account-controlled-maintained-by-microsoft-corp/) by territorial constraints. Several appeals followed, ultimately leading to the U.S. Supreme Court. The [central question throughout](https://www.lawfareblog.com/microsoft-ireland-case-supreme-court-preface-congressional-debate) was whether data stored outside of U.S. borders, but belonging to U.S. companies, was still subject to law enforcement warrants – and, relatedly, whether the invasion of privacy approved by a warrant took place in the United States or, in this case, Ireland. 

Before the Supreme Court case was decided, the U.S. Congress [passed updated legislation as part of an omnibus spending bill](https://www.theverge.com/2018/3/22/17131004/cloud-act-congress-omnibus-passed-mlat) that clarified that U.S. cloud service providers were indeed subject to U.S. law enforcement warrants, even if their data was [stored elsewhere](https://en.wikipedia.org/wiki/CLOUD_Act):

> Primarily the CLOUD Act amends the Stored Communications Act (SCA) of 1986 to allow federal law enforcement to compel U.S.-based technology companies via warrant or subpoena to provide requested data stored on servers regardless of whether the data are stored in the U.S. or on foreign soil.

Although in many cases these situations would be handled by [mutual legal assistance treaties](https://en.wikipedia.org/wiki/Mutual_legal_assistance_treaty), the main takeaway from the court case is that – as long as data is being stored by a provider with U.S.-based business interests – it is subject to U.S. law enforcement no matter where in the world the data is located. Practically all of the major IT vendors, systems integrators, and management consulting companies that work with the Canadian government also have U.S.-based operations.

## Operational security, not theatre

Data residency is a common myth because it intuitively _seems_ like data hosted in Canada will be more secure than data hosted elsewhere. The data residency myth becomes [a placeholder for more informed technical discussions](https://sboots.ca/2020/02/04/perils-of-standardization/#a-placeholder-for-more-informed-technical-discussions) – discussions that can quickly become deeply complex, relating to specific encryption techniques and cloud security best practices. 

There _are_ important questions that teams and organizations should be asking when they’re considering new cloud tools, including: 

* Is the service provider sharing your data with third parties? 
* What data export options are available, how comprehensive are they, and how easy would it be to switch to a competing service in the future? 
* What security and account management settings are available? Are they sufficient? 

All of these questions help determine how secure and effective a service is, but none of them have to do with where the service’s data is geographically stored.

In public service environments with [a shortage of technical expertise](https://sboots.ca/2020/01/02/bridging-the-technology-policy-gap/), simple explanations (like storing data in Canada to keep it safe) are attractive and reassuring. Data residency is “[security theatre](https://www.schneier.com/essays/archives/2009/11/beyond_security_thea.html)” because it gives the impression of making things secure, without actually adding any operational security benefits.

Data residency requirements do have some potential value when it comes to specific legal questions – namely, where lawsuits between a service provider and customer might take place, although this is usually determined in terms and conditions or contract details instead. And, as the Microsoft Ireland court case shows, unless the contract is with a company that has no U.S. business whatsoever, any information the company stores is still subject to U.S. law enforcement.

Ultimately, this is okay (or at the least, inevitable). Protected B information, mentioned above, isn’t meant to be secure from motivated foreign intelligence actors; there are other classification levels (and other networks) for information that genuinely should be protected from foreign eavesdropping. 

Government teams should focus their efforts on security and cloud infrastructure best practices – operational best practices, as opposed to compliance paperwork – and they should use the best cloud service providers available for their use-case, regardless of whether data is stored in the United States or not.

## Change for the better

Next week, updates to the main Government of Canada policy on information technology are coming into force, as the [Policy on Management of Information Technology](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=12755) is replaced by the [Policy on Service and Digital](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=32603). Among other changes – making the policy more streamlined and more closely focused on user needs – the update **removes** the formal data residency requirements that were previously included. 

The existing policy (being withdrawn on April 1, 2020) included the following language:

> Ensuring that all sensitive electronic data under government control, that has been categorized as Protected B, Protected C or is Classified, will be stored in a GC-approved computing facility located within the geographic boundaries of Canada or within the premises of a GC department located abroad, such as a diplomatic or consular mission. This does not mean that the country of origin of IT service providers must be Canada, as long as these service providers can ensure storage of data within boundaries or premises as described above.

The new policy is reorganized slightly, with departmental CIO responsibilities being moved to the accompanying [Directive on Service and Digital](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=32601). The corresponding language (emphasis mine) is,

> Ensuring computing facilities located within the geographic boundaries of Canada or within the premises of a Government of Canada department located abroad, such as a diplomatic or consular mission, **be identified and evaluated as a principal delivery option** for all sensitive electronic information and data under government control that has been categorized as Protected B, Protected C or is Classified.

This is a really welcome change, and opens the door to a much broader adoption of software-as-a-service tools than were previously available. 

It’s worth noting that some other Canadian government policies have not yet been updated to match this change – notably, the [Standards for the Conduct of Government of Canada Public Opinion Research](https://www.tpsgc-pwgsc.gc.ca/rop-por/enligne-online-eng.html#s13.2) (which still include explicit data residency requirements) and the 2017 [Direction for Electronic Data Residency](https://www.canada.ca/en/government/system/digital-government/modern-emerging-technologies/direction-electronic-data-residency.html) (which predates the policy requirements above but has not yet been formally deprecated). And, several provincial governments – namely British Columbia and Ontario – have provincial legislation that imposes data residency requirements for personal information and health data.

(Also worth noting – and it’s a topic where the terms often get mixed together – is the concept of **data sovereignty**, which is the ownership and hosting of data by Indigenous groups and other historically-marginalized communities. In an environment where social and cultural research has often been done _to_ marginalized groups rather than _with_ them, it’s a useful tool to rebalance power dynamics. You can learn more from this [Animikii article](https://www.animikii.com/news/decolonizing-digital-contextualizing-indigenous-data-sovereignty) or from the [First Nations Information Governance Centre](https://fnigc.ca/).)

As government technology practitioners, we operate in an environment with a long list of constraints – on how we work, what tools we use, and what permissions we need [to build and ship](https://sboots.ca/2020/01/10/shipping/) software and services. My goal, with blog posts like this one, is to remove as many constraints as I can – and to give people the space and trust to choose the tools that work best for them. 

Use the tools that work best for you. Think carefully about the (genuine) security and privacy implications of the tools you use, but don’t choose them based on security theatre and myths. Choose them because they’re the best tools.
