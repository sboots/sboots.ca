---
title: "Is this blocked in my department: a year in review"
date: 2021-01-04T18:41:39-07:00
summary: "Over the past year, departments have made a lot of progress in improving access to online collaboration tools and other services. But, there’s still a pretty dramatic gap between departments that are more restrictive, and departments that are more forward-looking. “Is this blocked in my department?” is a crowd-sourced effort to track that gap, and this post looks at how the website and the departments reflected on it have evolved over the course of 2020."
images: ["/img/2021/most-and-least-improved-departments-cropped.png"]
---

In my post [last week](/2020/12/27/tools-that-work/) I talked about how access to tools – online services, software, and modern computers – [will affect where public servants choose to work](/2020/12/27/tools-that-work/). Given a choice of organizations to work at, talented public servants [are](https://twitter.com/CalvinR/status/1345094544195538944) [going](https://twitter.com/meganiyoung/status/1344731328487546880) [to](https://twitter.com/patlaj/status/1345448307871641600) [choose](https://twitter.com/AvalinaCorazon/status/1330718223004786690) the departments and agencies that provide them with the best enabling environment. 

Over the past year, public servants across Canada adapted to working through the pandemic. Departments made [a lot of progress](/2020/05/22/crisis-bureaucracies-and-change/) in improving access to online collaboration tools and other services. But, there’s still a pretty dramatic gap **between departments** – the working environment for public servants in more restrictive departments is very different from that of their colleagues in more forward-looking departments.

One of the civic tech projects that I’ve maintained for a few years – **[Is this blocked in my department?](https://isthisblockedinmydepartment.ca/)** – is an effort to track that gap. It’s a crowd-sourced website where public servants can anonymously document the online services and other tools that they can or can’t access within their department. I built it in 2018 as an [Ottawa Civic Tech](https://ottawacivictech.ca/) project, and [soft-launched it](https://twitter.com/sboots/status/1080462696741588992) around this time in 2019. Seeing data come in over the past couple years [as people make suggestions](https://isthisblockedinmydepartment.ca/suggest) has really been a highlight. 

When the pandemic started, friends and colleagues across the federal public service [began using it](https://twitter.com/sboots/status/1238551530904715264) to figure out which of their counterparts in other departments they could communicate with, with which online services. Below is a quick look back at 2020 based on statistics from [Is this blocked in my department](https://isthisblockedinmydepartment.ca/). Happy new year, everyone! 

## Traffic by month

As you can guess, traffic to the website peaked pretty significantly in March, alongside the government’s very rapid shift to working from home. A couple weekends into March, I also built “[Should it be blocked in my department?](https://shoulditbeblockedinmydepartment.ca/)” (based on [a tweet from Imraan Bashir](https://twitter.com/iBashX/status/1238865058135932935)) which elaborates a bit on why public servants should be able to access online tools, and how to make the case for them if they’re unavailable. 

Traffic to both websites seems to be pretty heavily-driven by social media conversations (on [Twitter](https://isthisblockedinmydepartment.ca/service/twitter/), [LinkedIn](https://isthisblockedinmydepartment.ca/service/linkedin/), and discussion platforms like [GCcollab](https://isthisblockedinmydepartment.ca/service/gccollab/)).

<figure>
  <img src="/img/2021/pageviews-by-month.png" class="img-fluid" alt="A stacked bar chart of website pageviews by month for both “Should it be blocked in my department” and “Is this blocked in my department”. The chart peaks in March 2020, just shy of 2,700 pageviews. Other months average around 1,000 pageviews, with a decline in the summer that then ramps up again in September and October.">
  <figcaption><span class="sr-only">Caption: </span>Pageviews by month. <a href="https://github.com/isthisblocked/analysis/blob/main/2020/pageviews_by_month.csv">Source data <span class="sr-only">for pageviews by month</span></a></figcaption>
</figure>

## Submissions by month

People can make suggestions to Is this blocked using [one of four different Google Forms](https://isthisblockedinmydepartment.ca/suggest), depending on what kind of information they’re providing:

*   [Department-wide updates \
](http://bit.ly/isthisblocked-updates)To suggest changes for more than one service within a specific department
*   [Specific service updates \
](http://bit.ly/isthisblocked-individual)To quickly suggest changes for an individual service within a department
*   [Add a new service \
](http://bit.ly/isthisblocked-add-service)To suggest a new online service (collaboration tools, messaging platforms, etc.) to add to the dataset
*   [Add a new department \
](http://bit.ly/isthisblocked-add-organization)To suggest a federal department or agency to add to the dataset

In 2020, crowd-sourced submissions also peaked in March, but they were actually significantly less frequent than in 2019 (72 entries in 2020 versus <span title="Yes, 219 entries in 2019 is kind of a funny coincidence.">219</span> entries in 2019, across all four Google Forms).

<figure>
  <img src="/img/2021/submissions-by-month.png" class="img-fluid" alt="A stacked bar chart of crowd-sourced data submissions to “Is this blocked” by month, across three forms: “Add a new service suggestions”, “Department-wide updates”, and “Individual service updates”. The chart peaks in March 2020 just shy of 20 submissions that month; the other months are almost all below 5 entries per month, except for January, February, and June.">
  <figcaption><span class="sr-only">Caption: </span>Crowd-sourced data submissions by month. <a href="https://github.com/isthisblocked/analysis/blob/main/2020/submissions_by_month.csv">Source data <span class="sr-only">for submissions by month</span></a></figcaption>
</figure>

In 2020, there weren’t any submissions to the “Add a new department” form.

(It’s worth noting that – because data is anonymously submitted, and because I can’t double-check submissions by, for example, testing them on computers and networks in any department except the one I work for – there isn’t any kind of validation on the crowd-sourced submissions. So far I haven’t seen anything that looks like a deliberate attempt to skew departments’ results, which is nice! I manually update [the website’s dataset](https://github.com/isthisblocked/isthisblockedinmydepartment.ca/blob/master/src/data/organization_status.csv) based on the responses to these forms.)

## Submissions by department

Based on the same form data, here’s the top 20 departments by number of crowd-sourced submissions:

<figure>
  <img src="/img/2021/submissions-by-department.png" class="img-fluid" alt="A horizontal bar chart of crowd-sourced data submissions by department; the Treasury Board Secretariat is highest at 7, followed by Transport Canada, National Defence, the Canada School of Public Service, and Canada Revenue Agency all at 5 each. The other departments have less than 5 entries each.">
  <figcaption><span class="sr-only">Caption: </span>Crowd-sourced data submissions by department. <a href="https://github.com/isthisblocked/analysis/blob/main/2020/submissions_by_department.csv">Source data <span class="sr-only">for submissions by department</span></a></figcaption>
</figure>

This is based on submissions to both the “Department-wide updates” and “Individual service updates” forms.


## Highest- and lowest-scoring departments

Based on [the current dataset](https://github.com/isthisblocked/isthisblockedinmydepartment.ca/blob/master/src/data/organization_status.csv) (at the end of 2020), here’s the top 5 and bottom 5 departments and agencies, based on their [overall score](https://isthisblockedinmydepartment.ca/scoring). A few new services were added this year (bringing the total [from 35 to 38](https://isthisblockedinmydepartment.ca/service)), which brings the highest possible score – open access to every service in the list – from 105 to 114.

<figure>
  <img src="/img/2021/highest-and-lowest-scoring-departments.png" class="img-fluid" alt="A horizontal bar chart of the five highest and five lowest scoring departments. Transport Canada has the best score, at 112. Atlantic Canada Opportunities Agency and Parks Canada are next best. At the bottom end, the Royal Canadian Mounted Police has a score of minus 13, and FINTRAC has the second-lowest score at minus 1.">
  <figcaption><span class="sr-only">Caption: </span>Highest- and lowest-scoring departments. <a href="https://github.com/isthisblocked/analysis/blob/main/2020/highest_and_lowest_scoring_departments.csv">Source data <span class="sr-only">for highest- and lowest-scoring departments</span></a></figcaption>
</figure>

The five highest-scoring departments above ([Transport Canada](https://isthisblockedinmydepartment.ca/organization/tc/), [Atlantic Canada Opportunities Agency](https://isthisblockedinmydepartment.ca/organization/acoa/), [Parks Canada](https://isthisblockedinmydepartment.ca/organization/pc/), [Department of Justice](https://isthisblockedinmydepartment.ca/organization/justice/), and [Innovation, Science, and Economic Development Canada](https://isthisblockedinmydepartment.ca/organization/ic/)) are also the only five departments with a score above 103, which is 90% of the highest possible score. 

The [scoring system](https://isthisblockedinmydepartment.ca/scoring) is a bit arbitrary, but it was designed to avoid penalizing departments that were simply missing data when the site first launched. You can sort departments by highest and lowest score [on the Is this blocked homepage](https://isthisblockedinmydepartment.ca/).

## Most- and least-improved departments

One aspect I’ve been really interested to see is which departments improve the most, regardless of their starting point last year. Any progress departments make (opening up even a single service that was previously blocked) is something to celebrate. 

The departments below are the five most-improved and five least-improved departments; the number overlaid on each row is the positive or negative score change between the dataset a year ago and now. (Specifically, between [the Dec. 31, 2019 update](https://github.com/isthisblocked/isthisblockedinmydepartment.ca/blob/fb84e879ac7748f34e5276071340bc4303a4f643/src/data/organization_status.csv) and [the most recent update from Dec. 8, 2020](https://github.com/isthisblocked/isthisblockedinmydepartment.ca/blob/def2bc801eb54e08c849d44a00000a8a17ff99be/src/data/organization_status.csv).) 

<figure>
  <img src="/img/2021/most-and-least-improved-departments.png" class="img-fluid" alt="A bar chart that compares the 2019 and 2020 scores of the departments that improved the most and improved the least. The Department of Justice improved by +39, the Royal Canadian Mounted Police (despite its low overall score) improved by +24. The Canadian Nuclear Safety Commission went down by minus 5, and Library and Archives Canada went down by minus 4.">
  <figcaption><span class="sr-only">Caption: </span>Most- and least-improved departments. <a href="https://github.com/isthisblocked/analysis/blob/main/2020/most_and_least_improved_departments.csv">Source data <span class="sr-only">for most- and least-improved departments</span></a></figcaption>
</figure>

This chart excludes departments that didn’t have any data in 2019, and departments that didn’t have any new updates submitted in 2020. 

Only two departments “went backwards” (blocking more services in 2020 than in 2019); [Library and Archives Canada](https://isthisblockedinmydepartment.ca/organization/lac/) and the [Canadian Nuclear Safety Commission](https://isthisblockedinmydepartment.ca/organization/cnsc/). Despite the [Royal Canadian Mounted Police](https://isthisblockedinmydepartment.ca/organization/rcmp/)’s low overall score, it improved substantially between 2019 and now.

In each of these cases, whether this represents new firewall rules being introduced or changed, or just new crowd-sourced submissions that make the data more accurately reflect what was already in place, can’t be determined from the crowd-source submissions.

## What’s next?

Unlike other past civic tech projects ([putting the Internet Red Tape Reduction report online](https://internal-red-tape-reduction-report.github.io/), [analyzing Government of Canada contract spending](https://goc-spending.github.io/), or [building the Meeting Cost Calculator](https://meetingcostcalculator.ca/)), Is this blocked is a continually-growing and evolving website. In 2021, I hope it keeps on being useful to people as they communicate and collaborate with public servants in other departments, and as they think about which departments they’d want to work at next. 

Is this blocked is only as useful as the data that’s on it; if you see any errors or missing entries on the site, please [send in your suggestions](https://isthisblockedinmydepartment.ca/suggest)! You can also see how the website is built [by visiting the GitHub repository for the project](https://github.com/isthisblocked/isthisblockedinmydepartment.ca). 

Have a great 2021 and stay safe out there! 
