---
title: "A quick follow-up on digital identity"
date: 2022-06-16T11:14:41-07:00
summary: "A couple of months ago I wrote a post on my hopes for the future of digital identity in Canada. Most of the ideas I wrote were related to technical implementation details, but the broader theme was that I’d like to see the federal government play a bigger role, instead of deferring responsibility to provinces and territories."
images: []
---

A couple of months ago I wrote [a post on my hopes for the future of digital identity in Canada](/2022/04/21/small-hopes-for-the-future-of-digital-id-in-canada/). As someone who has lived in three different provinces and territories, and spent several years working outside of Canada, I have some thoughts on what I’d like it to look like! 

Most of the ideas I wrote were related to technical implementation details (to be [fast](/2022/04/21/small-hopes-for-the-future-of-digital-id-in-canada/#2-i-want-it-to-be-fast), to be [cross-department](/2022/04/21/small-hopes-for-the-future-of-digital-id-in-canada/#3-i-want-it-to-work-across-government-services-without-re-signing-in), to [work with my authenticator app](/2022/04/21/small-hopes-for-the-future-of-digital-id-in-canada/#4-i-want-it-to-work-with-my-authenticator-app)). The broader theme, though, was that I’d [like to see the federal government play a bigger role](/2022/04/21/small-hopes-for-the-future-of-digital-id-in-canada/#5-i-want-to-log-in-to-provincial-services-through-a-federal-id-not-the-other-way-around), instead of (as has historically been the case) deferring responsibility to provinces and territories. 

The post prompted a few responses, including two blog posts from [Michael Karlin](https://twitter.com/supergovernance) and [Tim Bouma](https://twitter.com/trbouma), respectively (two public servants that I’ve looked up to for years).

Michael’s piece looks at [the long history of policy and technical work done within the federal government on digital ID](https://medium.com/@supergovernance/the-long-road-of-digital-identity-16e8e497c895). It includes a great summary of why digital ID work in Canada is so hard:

> Identity information management is complicated in Canada. We have no national identity program so different orders of government have to share information about you regularly. If you were born in Canada, the authority of your identity information is the province of your birth. If you’re born outside of Canada, it’s the federal government via the information you provided during your immigration process. Provinces and territories share information between them as well; after all, many people don’t live in the province of their birth.

Michael’s look back at previous attempts (including those of his own team) is [an absolute must-read](https://medium.com/@supergovernance/the-long-road-of-digital-identity-16e8e497c895). It also helps explain how digital identity will likely (eventually) serve as the foundation for future online interactions well beyond government. And what the potential harms are if it’s done poorly, and a few ways of mitigating them.

Tim’s piece helps provide [an easy-to-understand introduction to what digital identity is](https://trbouma.substack.com/p/what-is-digital-identity?s=r).

> You’ll notice the word ‘trusted’ is an integral part of the definition. It’s one thing for you to have a digital identity to use, but it is entirely another thing for a federal program or service to trust that it is you using that digital identity and not someone else that is trying to be you. That’s why the definition of trusted digital identity was introduced, it must be trusted by government programs and services.
> 
> In the past, digital identity was conceptualized as very narrow IT-centric means of logging into a system or service with little regard to who you were as an individual. Fast forward to today, the concept of digital identity is evolving toward a more holistic view of what is actually needed by the individual so that they can have the best experience possible, without barriers, and in a way that empowers them.

Tim provides [a really great overview](https://trbouma.substack.com/p/what-is-digital-identity?s=r) of the current Government of Canada digital ID landscape, as well as efforts in the works by a variety of provinces.


## Politics has entered the chat

In the weeks after I wrote the earlier post, I was a bit surprised to see references to digital ID [show up in political news coverage](https://torontosun.com/opinion/columnists/furey-digital-ids-just-the-beginning-canadians-need-to-think-hard-about-these-issues). On the political right, there are concerns that digital ID programs would be used [to track people](https://www.itworldcanada.com/article/governments-must-fight-misinformation-on-digital-id-say-provincial-experts/479608), [their movements](https://paulwells.substack.com/p/we-need-to-talk-about-davos?s=r), or [their finances](https://twitter.com/Justin_Ling/status/1520476980998811648). In the meantime, the Saskatchewan government [announced that they were suspending work](https://www.cbc.ca/news/canada/saskatchewan/sask-digital-id-1.6405362) on a provincial digital ID.

As [a non-partisan public servant](/2020/01/21/principles-for-blogging-as-a-public-servant/), it’s often tempting to ignore the political landscape around our work entirely. Particularly for public servants working in technology modernization, our work tends to feel very politically-neutral: replacing old and fragile IT systems, trying to reduce costs, and trying to make government services easier to use are (by and large) goals that span across political divides. I often wish that political leaders across party lines [would pay _more_ attention to government technology issues](/2021/12/15/a-bleak-outlook-for-public-sector-tech/). (Too often, they’re seen as unimportant, boring, or niche, [despite their impact](/2020/02/25/our-services-arent-working/) on people, businesses, and public trust.)

For once, sort of unexpectedly, that has happened. Being aware of the political dialogue around digital ID (or any public sector technology topic that makes the news) is definitely useful. It would not surprise me if – after almost two decades without much progress – the federal public service finally makes some great strides on digital ID implementation, only to have it crash upon the rocks of unanticipated political opposition. For all we know, this might be what recently happened in Saskatchewan.

On the other hand, as Michael hints at [in his piece](https://medium.com/@supergovernance/the-long-road-of-digital-identity-16e8e497c895), there’s a longer-term danger that comes from governments ceding this field completely to unregulated and less accountable private sector companies, in everything from [authentication](https://twitter.com/caparsons/status/1443943480175304707) to [identity verification](https://www.wired.com/story/irs-drops-facial-recognition-verification/) to [age assurance](https://twitter.com/supergovernance/status/1533854454474227713).

What does this mean for digital ID efforts at the federal level? My advice would be [the same as in the original post from April](/2022/04/21/small-hopes-for-the-future-of-digital-id-in-canada/): **don’t start with digital ID at all**. Start with authentication. Build a robust, easy-to-use login system, something comparable to the US’s [login.gov](https://www.login.gov/). Make sure that it doesn’t accidentally exclude people. Use modern tech, test it extensively with everyday people, and roll it out across federal departments to replace the mishmash of current login systems.

Start small, build something that’s useful, and from there, keep going at the pace of public trust.

_For more on digital ID, [Public Digital’s series of blog posts](https://public.digital/blog/tag/identity) from the UK is excellent._
