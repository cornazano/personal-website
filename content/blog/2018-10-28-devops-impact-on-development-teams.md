---
date: 2018-10-28
title: "DevOps Impact on Development Teams: Open spaces discussion at DevOpsDays Montreal"
summary: >
  2018-10-28.
  Summary of the DevOpsDays Montreal open space discussion about what it takes to move a team from Dev to DevOps.
---

As traditional development teams become more operationally aware and adopt practices such as CI/CD, how do their development habits and work management processes need to change?

This was the leading question for a discussion during the Wednesday open spaces at DevOps Days Montreal. I was interested in the topic because we've seen impacts on both of these fronts in my team at work over the past three years, and I wanted to hear what other people were experiencing. The discussion eventually covered three different types of impacts: developer mindset, pipelines, and work management.

---

A traditional developer mindset frequently involves developing in a feature branch, and seeing the entire feature one merge request for review purposes. As we move to trunk-based development and frequent merges, the way we think about changes needs to adjust as well. Two types of challenges were raised during the discussion:

* Developers may not see the point of merging (currently) unused code.
* Developers may be shy about pushing to master.

For people accustomed to batching all the changes for a feature into a "final" version before showing the work to their colleagues, it will take experience with the trunk-based development and continuous integration practices before they become comfortable with it.

---

Delivery pipelines were also raised as an obstacle that will be faced while navigating the shift to DevOps practices. Long testing times and gated processes with multiple builds can impede frequent integration. (A way of viewing this that wasn't raised during the discussion: long cycle times can increase the per-transaction cost for each integration, which pressures us to use larger batch sizes.) Two potential optimization strategies were discussed to address this: replacing the remaining manual steps with automation into a more continuous pipeline, and shifting from rebuilding artifacts at different stages to a build-once-then-promote approach.

The development team needs to invest more in their delivery pipelines than they may be accustomed to when working with slower release cadences. Ongoing tests and code reviews are important as a foundation for making changes safe, especially if there is user data maintained by the systems we're operating.

---

How we manage work - and even what we think of as being our work - needs to shift as we adopt a DevOps perspective and practices. Using feature branches, we may be accustomed to thinking of the relationship between JIRA cards and checkins / merges to master as being in a one-to-one relationship. Trying to maintain this while moving to a model where we merge into master multiple times per day doesn't scale; there needs to be a looser coupling between the two, where individual checkins don't matter in JIRA.

A really good remark was that the team's definition of DONE should shift from the point where code is merged to include having the code being deployed into the live production environment. My personal experience is that this still a gap, where the code may be in production but remain unused, delivering no value. My team at work has included deployment to production in our definition for a few years already, and we're working on shifting to DONE including the organization deriving benefit from the work.

Ultimately, it's about your team's process and what helps you develop faster flow and more effective feedback mechanisms.

**_Thank you to everyone who participated in this discussion._**
