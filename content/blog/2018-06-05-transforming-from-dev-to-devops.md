---
date: 2018-10-28
title: "Transforming from Dev to DevOps: Open spaces discussion at DevOpsDays Toronto"
summary: >
  2018-10-28.
  Summary of the DevOpsDays Toronto open space discussion about moving from Dev to DevOps.
---

How do we lead a traditional development team through a transition to a devops-oriented ownership of the services they build?

This is a transition my team at work has been going through for a couple of years now. To get a wider perspective on what other people are encountering on similar journeys, I proposed this as an open spaces topic at DevOps Days Toronto last Thursday. About 30 people show up to discuss it and share their experiences. Here are some of the main points raised during the session.

Establish a Learning Culture
--------------------------------------------------------------------------------

Owning a service requires a team to have a wider knowledge base than a traditional development team. An important cultural element is to ensure that team members continue to learn and develop the skills the team needs.

A key step here is to make it visible that people are taking time for self improvement - and that there is an expectation that they are taking that time. Some techniques that can be used to encourage this include:

* book clubs / reading groups;
* project presentations;
* meetup talks; and
* dedicated learning time.

Everyone should be encouraged to attend and participate in these types of activities, and preparation for them should be part of the job.

Organize for Feedback and Support
--------------------------------------------------------------------------------

In a traditional development context, team members may not need to pay much attention to what actually happens in production environments. As a team increases their degree of ownership of a service, they need to get to a point where the developers care about what happens in production.

Much of this will depend on the feedback loops they establish within the organization. If developers have typically only had direct exposure to test outputs and QA feedback, start contributing responses to support requests. Developing an on call policy for the team will get the team even more involved in understanding what happens when their code encounters real operational conditions.

A frequent benefit of these improved feedback loops is that the developers will be able to make better choices about what information to log, which metrics to collect, and what monitoring is needed. These choices will be especially important in establising sustainable SLAs and alerting policies. Making sure that people aren't getting woken up unless there are actual business-affecting issues is important.

Manage Incidents
--------------------------------------------------------------------------------

As teams take more ownership of the services they build, team members will end up being more involved with incident management and resolution.

The specifics of how incidents are managed will vary a bit depending on the on call policy that the team has established. One example that was discussed was a team that has their more experienced developers handle the overnight on call responsibilities. With this policy, incidents are handled slightly differently depending on whether they occur during normal working hours:

If the incident is outside of normal working hours, the developer on call handles the incident, and then the team as a whole is involved in the more detailed investigation that happens the following morning.

If the incident occurs during working hours, the team works on the incident together. This helps develop less experienced team members abilities, contributing to their ongoing learning and preparation for future on call responsibilities.

No matter what the exact policy is, contact information and incident procedures should be easily accessible by team members, and they should know where this information is.

Align Responsibilities and Compensation
--------------------------------------------------------------------------------

Owning the service, and inclusion of on call duties within a team, increase the team's responsibilities and their potential impact to the organization. While it isn't often in a team's immediate control, compensation should be considered during the transition.

The on call team member needs to be available when an incident occurs. One of the participants mentioned that this should be accompanied by a flat bump (set amount of additional pay) for being available, whether there are any calls or not.

When an incident occurs, the on call team member will actually end up working. A suggestion here is to compensate them with lieu time, essentially crediting them with a portion of the time they spent handling the incident as part of their hours for the week. This may be set up as something other than 1:1 - for example, they might get credited with 45 minutes of work time for each hour worked to resolve an incident outside of working hours.

Compensation policies like these may be able to acknowledge the contributions of the on call team members without incentivizing undesired behaviors.

**_Thank you to eveyrone who particpated in the discussion, sharing your ideas and experiences._**
