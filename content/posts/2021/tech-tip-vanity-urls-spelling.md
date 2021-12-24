---
title: "Public service tech tip: If you create “vanity URLs”, expect people to spell them wrong"
date: 2021-12-24T11:35:14-05:00
summary: "If you’re working in government communications, you’ve probably come across “vanity URLs” before. These are easily-written-out shortcuts to webpages that typically have longer, more complex web addresses. You’ll often see them in TV or online advertisements, spoken out on radio ads, or included on billboards, posters, and other printed communications. With vanity URLs, people are frequently typing them in “by hand”, in the address bar of their web browser. That’s partly why they’re so useful, but it also means that people are likely to type them incorrectly."
images: ["/img/2021/canada-ca-covid-vaccine-youtube.jpg"]
---

If you’re working in government communications, you’ve probably come across “vanity URLs” before. These are easily-written-out shortcuts to webpages that typically have longer, more complex web addresses. You’ll often see them in TV or online advertisements, spoken out on radio ads, or included on billboards, posters, and other printed communications. They’re really handy. 

<figure>
  <img src="/img/2021/canada-ca-covid-vaccine-youtube.jpg" class="img-fluid" alt="A screenshot from a Youtube and television advertisement published by the Public Health Agency of Canada. It shows a teacher and student taking a selfie next to a school bus on the left, and the text “Learn more at Canada.ca/covid-vaccine” on the right. In small text at the bottom it says, “Vaccinated or not, follow local guidelines for gatherings and public health measures.”.">
  <figcaption><span class="sr-only">Caption: </span>An example of a vanity URL for the <a href="https://www.canada.ca/en/public-health/services/diseases/coronavirus-disease-covid-19/vaccines.html">Government of Canada’s webpage on COVID-19 vaccines</a>. <a href="https://www.youtube.com/watch?v=TkaiXadCukA">Source: YouTube</a></figcaption>
</figure>

Vanity URLs are a standard part of the [Government of Canada’s web communications guidelines](https://www.canada.ca/en/treasury-board-secretariat/services/government-communications/canada-content-information-architecture-specification/organizing-content.html#toc3). They’re just another name for [redirects](https://en.wikipedia.org/wiki/URL_redirection), which have been around since the [early days of the web](https://datatracker.ietf.org/doc/html/rfc2616#section-10.3.2). 

The name “vanity URL” seems to originate [from the Adobe content management system](https://helpx.adobe.com/ca/experience-manager/kb/vanity-urls.html) that powers Canada.ca (although other systems and providers occasionally also use the term). It’s a bit of a weird name (“are these URLs …vain?”).  I usually just call them “redirects”, going back to the start of my web developer days, but I’ll use “vanity URLs” in this post.

What’s noteworthy about vanity URLs is that – unlike links that are shared in emails or other webpages – **people are frequently typing them in “by hand”**, in the address bar of their web browser. That’s partly why they’re useful (and more useful the shorter and more memorable they are). But it also means that people are very likely to type them incorrectly. That’s something worth planning for. 

Whenever I see a vanity URL on a Canadian government advertisement or publication, I have a few immediate reactions:

* Does it still work if you type it without the hyphens?
* Are there any complicated words that (if you heard it spoken out, instead of written) you might mis-hear or spell wrong?
* If you only partly remember the URL later, how likely are you to get to the page you’re trying to reach?

If people type in a vanity URL that doesn’t exist, they’ll get an “Error 404” (page not found) message instead of the information you’re trying to help them reach. 

The solution is to create _a lot_ of vanity URLs, for all the different variations (and misspellings) of the main vanity URL that you plan on publicly communicating.

## A few examples

Let’s try that out in practice, on some URLs related to the Canadian government’s [COVID-19 -related information](https://www.canada.ca/en/public-health/services/diseases/coronavirus-disease-covid-19.html) (as of mid-December 2021; these might change in the future).

<table class="table table-striped table-bordered">
  <thead>
  <tr>
   <th><strong>URL</strong>
   </th>
   <th><strong>Does it work</strong>
   </th>
  </tr>
  </thead>
  <tbody>
  <tr>
   <td><a href="https://canada.ca/covid-19">canada.ca/covid-19</a>
   </td>
   <td>Works ✅
   </td>
  </tr>
  <tr>
   <td><a href="https://canada.ca/covid19">canada.ca/covid19</a>
   </td>
   <td>Works ✅
   </td>
  </tr>
  <tr>
   <td><a href="https://canada.ca/covid">canada.ca/covid</a>
   </td>
   <td>Does not work ❌
   </td>
  </tr>
  <tr>
   <td><a href="https://canada.ca/covid-vaccines">canada.ca/covid-vaccines</a>
   </td>
   <td>Works ✅
   </td>
  </tr>
  <tr>
   <td><a href="https://canada.ca/covidvaccines">canada.ca/covidvaccines</a>
   </td>
   <td>Works ✅
   </td>
  </tr>
  <tr>
   <td><a href="https://canada.ca/covid-vaccine">canada.ca/covid-vaccine</a>
   </td>
   <td>Works ✅
   </td>
  </tr>
  <tr>
   <td><a href="https://canada.ca/covidvaccine">canada.ca/covidvaccine</a>
   </td>
   <td>Works ✅
   </td>
  </tr>
  </tbody>
</table>

All told, that’s a pretty good track record – hat tip to our public health communication folks! 

If your team or project is using a vanity URL, you can try the same exercise: add or remove hyphens, say it out loud (and think about how people hearing it on the radio might register it), and think of different synonyms or words that people might _think_ they saw or heard when your vanity URL briefly passed them by. (And do all this in both official languages, of course!)

I’d be curious how many people land on the “Error 404” page for [canada.ca/covid](https://canada.ca/covid), and if there are web analytics stats that are available to comms teams to help them identify where new vanity URLs could be created. Some content management systems [can be set up to send automatic alerts](https://www.drupal.org/project/notify_404) in this case.  If you’re seeing a large number (or even a small number!) of Error 404s on a particular URL, that’s a great reason to add a new vanity URL at that exact address. 

When webpages get moved from one location to another, it’s also really valuable (dare I say, morally important) to add redirects so that people going to the old addresses can find the new ones. As Tim-Berners Lee (the [inventor of the World Wide Web](https://en.wikipedia.org/wiki/Tim_Berners-Lee)) would say: [cool URLs don’t change](https://www.w3.org/Provider/Style/URI). If you’re moving where something lives on the internet, make sure that people can immediately make their way to the new location. That’s something the Canadian government [hasn’t historically been great at](/2021/10/24/if-its-not-public-does-it-even-matter/). 

What’s the takeaway? If you create vanity URLs, don’t just create one or two; create _a bunch_ that are all designed to account for different ways that people could mis-spell or mis-hear your main vanity URL. If someone ends up on an “Error 404” page instead of your content, they’re probably going to just give up instead of trying another variation of the address they typed in. You’ve written good stuff – help people find it every possible way they can. 

{{% manualrelatedposts title="More public service tech tips:" %}}
- [Paste without fonts and formatting](/2020/09/18/public-service-tech-tip-paste-without-fonts-and-formatting/)
- [Please use headings](/2020/01/14/public-service-tech-tip-please-use-headings/)
{{% /manualrelatedposts %}}
