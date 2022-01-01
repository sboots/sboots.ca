---
title: "Is this blocked in my department: 2021 year in review"
subtitle: "Spotify Wrapped but for “can I actually use this website at work?”"
date: 2022-01-01T01:31:46-05:00
summary: "Using online collaboration tools has been a big part of making it possible for federal public servants to work from home during the pandemic. That’s a big change for Government of Canada departments, who have historically been very reluctant to allow access to these tools. Since 2019, I’ve tracked where online services are allowed or blocked at “Is this blocked in my department.ca”, with anonymous submission forms that let people report which sites they can access in each department. Here, for the second year running, is the 2021 “Is this blocked in my department” year in review."
images: ["/img/2022/itb-cover.png"]
---

Another year has gone by, and it’s been a weird one. The pandemic is [still very much happening](https://buttondown.email/lchski/archive/hit-and-miss-224-staring-down-the-barrel-at-least/), and most federal public servants are still working from home.

Using online collaboration tools has been a big part of making it possible to work from home. That’s a big change for Government of Canada departments, who have historically been very reluctant to allow access to these tools. Since 2019, I’ve tracked where online services are allowed or blocked at [Is this blocked in my department.ca](https://isthisblockedinmydepartment.ca/), with a set of [anonymous submission forms](https://isthisblockedinmydepartment.ca/suggest) that let people report which sites they can access in each department.

Below is the 2021 “Is this blocked in my department” year in review; you can [read the 2020 year in review here](/2021/01/04/is-this-blocked-in-my-department-a-year-in-review/).


## Traffic by month

Like last year, traffic to the website varied quite a bit from month to month based on social media coverage. In 2021, “Is this blocked” had 10,600 pageviews, compared to 11,500 in 2020. Similarly, the [“Should it be blocked in my department” companion site](https://shoulditbeblockedinmydepartment.ca/) had 1,800 pageviews in 2021 compared to 2,000 pageviews in 2020.

{{% figurecaption src="/img/2022/itb-pageviews-by-month.png" alt="A stacked bar chart of website pageviews by month for both “Should it be blocked in my department” and “Is this blocked in my department”. The chart is highest in January, March, and December 2021, with around 2,000 pageviews for each of those months (cumulatively across both websites). Throughout the rest of the year, traffic is generally between 500 and 1,000 pageviews per month." caption="Pageviews by month." url="https://github.com/isthisblocked/analysis/blob/main/2021/pageviews_by_month.csv" urltext="Source data" urlextratext=" for pageviews by month" %}}


## Submissions by month

Data for each department is submitted anonymously by public servants, using [one of the four suggestion forms](https://isthisblockedinmydepartment.ca/suggest). In 2021, people sent in 108 suggested updates, more than the 72 updates sent in in 2020.

This included 11 suggestions for new services, and 5 suggestions to add new departments and agencies. 

All five of these organizations have now been added; if you sent in a request to add a new department, be sure to come back and send in an update on which services are available or blocked in that department!

{{% figurecaption src="/img/2022/itb-submissions-by-month.png" alt="A stacked bar chart of crowd-sourced data submissions to “Is this blocked” by month, across four forms: “Add a new organization suggestions”, “Add a new service suggestions”, “Department-wide updates”, and “Individual service updates”. The chart peaks in January 2021 just shy of 25 submissions that month; the next several months are all quite low. From September onwards, there are about 15 submissions each month." caption="Crowd-sourced data submissions by month." url="https://github.com/isthisblocked/analysis/blob/main/2021/submissions_by_month.csv" urltext="Source data" urlextratext=" for submissions by month" %}}

## Submissions by department

Not counting suggestions to add a new service or to add a new organization, there were 92 suggested updates to data for specific departments.

{{% figurecaption src="/img/2022/itb-submissions-by-department.png" alt="A horizontal bar chart of crowd-sourced data submissions by department; Infrastructure Canada is highest at 10, followed by Statistics Canada at 7. Several departments have about 5 submissions each, while the “Other departments and agencies” category at the end has 16. " caption="Crowd-sourced data submissions by department." url="https://github.com/isthisblocked/analysis/blob/main/2021/submissions_by_department.csv" urltext="Source data" urlextratext=" for submissions by department" %}}

The quality of the data gets better the more submissions are sent in. Big thanks to everyone who contributed updates in 2021!


## Highest- and lowest-scoring departments

As new services were added to the dataset, the highest possible score (for 100% services open by default) increased from 114 last year to 129 this year.

[Transport Canada](https://isthisblockedinmydepartment.ca/organization/tc/) retained its 2020 title, as the highest-scoring department in 2021 as well. **Congrats to everyone at TC who worked on opening up access to modern tools in the department!** [Parks Canada](https://isthisblockedinmydepartment.ca/organization/pc/) moved from third place last year to second place this year, while [Veterans Affairs Canada](https://isthisblockedinmydepartment.ca/organization/vac/) and [Global Affairs Canada](https://isthisblockedinmydepartment.ca/organization/gac/) moved up into the top rankings. 

Several departments tied for fifth-highest place: [FedDev Ontario](https://isthisblockedinmydepartment.ca/organization/feddev/); [Innovation, Science and Economic Development Canada](https://isthisblockedinmydepartment.ca/organization/ic/); [Indigenous Services Canada & Crown-Indigenous Relations and Northern Affairs Canada](https://isthisblockedinmydepartment.ca/organization/inac/).

Not surprisingly, security-related departments and agencies tended to have the lowest scores, with the [Royal Canadian Mounted Police](https://isthisblockedinmydepartment.ca/organization/rcmp/) likewise retaining its last-place finish from last year:

{{% figurecaption src="/img/2022/itb-highest-lowest-scoring-departments.png" alt="A horizontal bar chart of the five highest and five lowest scoring departments. Transport Canada has the best score, at 127. Parks Canada and Veterans Affairs Canada are next best. At the bottom end, the Royal Canadian Mounted Police has a score of minus 15, and FINTRAC has the second-lowest score at minus 7." caption="Highest- and lowest-scoring departments." url="https://github.com/isthisblocked/analysis/blob/main/2021/highest_and_lowest_scoring_departments.csv" urltext="Source data" urlextratext=" for highest- and lowest-scoring departments" %}}


## Most- and least-improved departments

One of my favourite categories [from last year’s analysis](/2021/01/04/is-this-blocked-in-my-department-a-year-in-review/#most-and-least-improved-departments) was looking at which departments and agencies _improved_ the most (or least) since the previous year.

The five most-improved and five least-improved departments in 2021 are shown below; the number overlaid on each row is the positive or negative score change since last year. (Specifically between [the Dec. 8, 2020 update](https://github.com/isthisblocked/isthisblockedinmydepartment.ca/blob/def2bc801eb54e08c849d44a00000a8a17ff99be/src/data/organization_status.csv) and [the most recent update from Dec. 26, 2021](https://github.com/isthisblocked/isthisblockedinmydepartment.ca/blob/ab976d29effd25c99e89ff0ae956eb4b8a6d9194/src/data/organization_status.csv).)

{{% figurecaption src="/img/2022/itb-most-least-improved-departments.png" alt="A bar chart that compares the 2020 and 2021 scores of the departments that improved the most and improved the least. FedDev Ontario improved by +81; Indigenous Services Canada & Crown-Indigenous Relations and Northern Affairs Canada increased by +78; Elections Canada increased by +75. At the other end, the Department of Justice decreased by 2 to a score of 104, and the Royal Canadian Mounted Police decreased by 2 to a score of minus 15." caption="Most- and least-improved departments." url="https://github.com/isthisblocked/analysis/blob/main/2021/most_and_least_improved_departments.csv" urltext="Source data" urlextratext=" for most- and least-improved departments" %}}

Three departments had overall lower scores than last year: [Correctional Service Canada](https://isthisblockedinmydepartment.ca/organization/csc/); [Department of Justice Canada](https://isthisblockedinmydepartment.ca/organization/justice/); and the [Royal Canadian Mounted Police](https://isthisblockedinmydepartment.ca/organization/rcmp/).


## Most-frequently blocked and restricted services

New this year is a look at which online tools and services are the most likely to be blocked in departments. The top twenty most-frequently blocked and restricted services are shown below.

Although the main focus of “Is this blocked” is online services accessed through a web browser, installed software programs are also critical to the work of public servants. These programs show up fairly highly in the list of most-blocked services: [Skype](https://isthisblockedinmydepartment.ca/service/skype/) for videoconferencing, [Python](https://isthisblockedinmydepartment.ca/service/python/) and [R Studio](https://isthisblockedinmydepartment.ca/service/rstudio/) for data analysis, and the [Mozilla Firefox](https://isthisblockedinmydepartment.ca/service/mozillafirefox/) and [Google Chrome](https://isthisblockedinmydepartment.ca/service/googlechrome/) web browsers. 

The online services in the most-blocked list cover a wide range of use-cases, from videoconferencing to social media to document sharing and team collaboration. Over time, I hope this list gets smaller and smaller.

{{% figurecaption src="/img/2022/itb-most-frequently-blocked-services.png" alt="A horizontal bar chart showing the most-frequently blocked and restricted services. Skype is at the top, being restricted in 11 departments and blocked in 9 departments. Google Meet, Mozilla Firefox, Dropbox, and Python are next on the list. At the lower end, Facebook and GitHub are both restricted in 3 departments and blocked in 2 departments." caption="Most-frequently blocked and restricted services." url="https://github.com/isthisblocked/analysis/blob/main/2021/most_blocked_services.csv" urltext="Source data" urlextratext=" for most-frequently blocked and restricted services" %}}

Services that are marked as “restricted” in the data set include cases where only specific staff in a department can access the service (for example, only comms staff being able to access social media websites, or only IT staff being able to use data analysis tools). 

If there are several submissions from the same department that disagree, within a similar timespan, the “restricted” category is also used as a tie-breaker, since this situation usually indicates that access to the service is uneven across the department. “Restricted” is also used if staff need to request permission to access a service (for example by sending in an IT service ticket), rather than it being available by default. 

“Blocked” – where services aren’t available within a department at all, even when staff ask for them – is weighted twice as heavily as “restricted” in the chart above, since this situation is the most likely to significantly hamper public servants’ work.

**If you’re in an IT management, desktop services, or leadership role in a department, you should think seriously about making each of these services open by default.** Reducing barriers to using modern tools makes public servants more capable, more effective, and more productive. Not to mention: happier, and [more likely to want to work in your department](/2020/12/27/tools-that-work/)!


## To 2022!

I’m always thrilled to see new updates come in to [Is this blocked in my department](https://isthisblockedinmydepartment.ca/). If you’ve sent in suggestions over the past year, thanks so much for having made the site better! 

As always, if you see any errors or missing entries on the site, please [send in your suggestions](https://isthisblockedinmydepartment.ca/suggest)! If you have other thoughts or feedback, you can email [isthisblockedinmydepartment@gmail.com](mailto:isthisblockedinmydepartment@gmail.com) or give me a shout [on Twitter](https://twitter.com/sboots).

Please stay safe and healthy – happy new year to you and yours! 
