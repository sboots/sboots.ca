---
title: "How many Government of Canada services are online from start to finish?"
date: 2021-10-12T23:29:07-07:00
summary: "Getting accurate data on how many government services can be completed online is challenging. Even determining how many government services exist across a range of departments and agencies is often a struggle. Fortunately, in 2020, the Office of the CIO published a comprehensive update to the GC Service Inventory open data set – it’s really excellent. As a recent civic tech project, I put together an analysis website that dives into how many of those services can currently be completed online from end-to-end."
images: ["/img/2021/end-to-end-services-screenshot.png"]
featured: true
---

_**Update:** In December 2021, I updated the methodology [used in the end-to-end services analysis](https://end-to-end-services.github.io/#methodology). Following the update, services that are all “not applicable” are no longer counted as fully online. Overall, [19% of Government of Canada services are online end-to-end](https://end-to-end-services.github.io/), instead of 45%. This more closely matches [the official methodology recently published on the GC InfoBase website](https://www.tbs-sct.gc.ca/ems-sgd/edb-bdd/index-eng.html#infographic/gov/gov/services/.-.-(panel_key.-.-'services_digital_status))._

Back in early 2020 I wrote a blog post about [the quality of federal government services](/2020/02/25/our-services-arent-working/) (something that my career is by and large [dedicated to improving](/2020/01/02/bridging-the-technology-policy-gap/)!). It included a litmus test for government services: **can I complete this service online, on my phone, from start to finish, at two in the morning?**

Getting accurate data on how many government services meet that mark is challenging. It’s challenging for any government, not just Canada! Even determining how many government services _exist_ across a vast range of departments and agencies is a struggle. Although it was ([very](https://twitter.com/mattlane/status/1361489230166335488) [sadly](https://twitter.com/HimalMandalia/status/1362736671519866884)) decommissioned this past year, the [United Kingdom’s Performance platform](https://web.archive.org/web/20200303183932/https://www.gov.uk/performance) was one of the first and best efforts at doing this. It mapped out both how many services the government offered, and how effective they were at meeting a set of consistent performance criteria. UK digital government folks have also written [some](https://designnotes.blog.gov.uk/2015/06/22/good-services-are-verbs-2/) [great](https://hodigital.blog.gov.uk/2016/12/21/creating-a-common-language-to-describe-services/) [pieces](https://scottcolfer.com/2018/05/14/public-service.html) [on](https://twitter.com/b_schmittling/status/1323171864923942913) what a service _is_, which isn’t always a straightforward question.

In Canada, a team in the Treasury Board Secretariat’s Office of the CIO publishes the [GC Service Inventory](https://open.canada.ca/data/en/dataset/3ac0d080-6149-499a-8b06-7ce5f00ec56c), which lists each service offered by federal departments and agencies. Although it originally only included a handful of departments, the 2019-2020 update to the dataset included services from more than 70 departments and agencies, along with a range of indicators about each service. I was _very_ stoked to see this get [published publicly on the Open Government website](https://open.canada.ca/data/en/dataset/3ac0d080-6149-499a-8b06-7ce5f00ec56c), and I’m a huge fan of the team that produced it.

## Counting up end-to-end services

<figure>
  <img src="/img/2021/end-to-end-services-screenshot.png" class="img-fluid" alt="A screenshot of the “End-to-end services” analysis website, titled “How many government services are available online end-to-end in Canada?” and with an orange “45%” indicator below the heading, stating that 500 of the 1117 public-facing services in the GC Service Inventory are online from end-to-end.">
  <figcaption><span class="sr-only">Caption: </span>A screenshot of the “End-to-end services” analysis website. <a href="https://end-to-end-services.github.io/">Visit the site <span class="sr-only">to see a department-by-department analysis.</a></figcaption>
</figure>

Over the past couple weekends, I put together [a new civic tech website that analyzes the GC Service Inventory data and comes up with a tally of end-to-end services](https://end-to-end-services.github.io/), across the government and across each department or agency.

According to the 2019-2020 data, **45% of Government of Canada services are available from end-to-end**. That’s actually pretty solid, and quite a bit higher than I was expecting. This percentage varies fairly significantly from one department to the next, and it doesn’t factor in the _volume_ of service transactions (for example, a service used by hundreds of thousands of people each year is weighted the same as a service only used by a dozen). 

Services in the GC Service Inventory data set are also self-reported by departments, each of whom may have interpreted the [online interactions criteria](https://end-to-end-services.github.io/#methodology) (there are six) slightly differently. Hopefully this data set continues to improve and grow each year, as departments add any missing services.

Unlike some previous projects (mainly, [Is this blocked in my department?](https://isthisblockedinmydepartment.ca/)) I don’t have any solid ideas on how to gather feedback about any missing or inaccurate service entries. One approach would be a parallel, community-contributed data set (I’ve added a very basic Google Form option to suggest corrections to existing entries, but adding new services would be more complicated) and ideally there would be a clear mechanism to report issues to each department directly. If you have thoughts or suggestions I’d love to hear them!

You can [take a look at the methodology](https://end-to-end-services.github.io/#methodology) for more on how the site works, or the [GitHub repository](https://github.com/YOWCT/end-to-end-services) for technical details. [Check out the website](https://end-to-end-services.github.io/), see how your department stacks up, and [let me know](https://twitter.com/sboots) what you think!
