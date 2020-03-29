---
date: 2019-06-23
title: "Remote-First Work: Open spaces discussion at DevOpsDays Toronto 2019"
summary: >
  2019-06-23.
  Summary of the DevOpsDays Toronto open space discussion about how to make
  remote work _work_.
---

The week before DevOpsDays Toronto, I was able to attend some of the sessions at the [CALICO](https://calico.org) (Computer-Assisted Language Instruction Consortium) conference in Montreal. One of the sessions was a panel discussion on _Teaching Less Commonly Taught Languages in a Distance Environment_. They discussed a collaborative effort among three universities (Yale, Columbia, and Cornell) to develop and evaluate techniques for language instruction when the students are getting a real-time, classroom-oriented experience, but where some of the students happen to be gathered on a different campus than others.

While they didn't talk about remote work, the challenges they faced sounded a lot like what we face when working as distributed teams. This prompted me to propose an open spaces topic to explore and learn a bit more about dealing with remote work and remote-first approaches. The rest of this post is based on the discussion during the open spaces session, and hopefully captures the main points that were covered.

---

The people who showed up to the session came from a variety of organizations, ranging from very small companies (12 people) to large enterprises (10,000+ employees). Some of the participants were working almost entirely remotely, while others were working primarily with a co-located team.

What is remote work?
--------------------------------------------------------------------------------

When we start to think about remote work, there are two variants that can have different implications: _remote offices_ or _remote individuals_. Remote offices produce "clumps of co-located people", and the social dynamic is likely to be different than when we deal with the isolation that can occur for remote individuals. In the case of remote individuals, it may also be an intermittent thing - one of the participants mentioned that they have an office, but that on any given day roughly half of their team was working from home.

Working as a distributed team will create the same types of challenges in both variants, but the potential approaches to addressing them may need to be adapted to the differences between them. In all cases, working with a distributed team will require a move towards a _remote-first culture_ that actively supports the distributed team, and avoids collaboration techniques that only work locally.

Keeping team coherence
--------------------------------------------------------------------------------

When working effectively, a team is more than just a collection of individuals. This can be harder to maintain on a distributed team. One of the challenges is that remote colleagues - especially in the case of remote individuals - may end up being viewed as (or feel like) second-class citizens, excluded from the team. This can show up in various ways, ranging from social aspects (they're not at the pizza party) to more direct impediments to full participation (they're not in the hallway-track decision making process).

There are ways to reduce this effect. Consider, for example, a team pizza party in a central location. Holding it in a space with video conferencing allows remote people to participate. Even better, have them order pizza and expense it; this helps bring the team together with the shared activity. Bringing people in for face-to-face time is also important to developing good interpersonal relationships. [Note: this point was also raised by the panel at the CALICO conference. The instructor is based at one of the universities, and is required to travel and teach from the other ones where they have students.]

The more distributed a team is, the more important these choices become. Some of them are organizational, but others are things we control as individuals. Discussion participants suggested two good habits to develop when working remotely. The first is to make sure you connect regularly, to ensure people don't forget you're there. The second is to turn on your camera so that people remember who you are.

Process visibility
--------------------------------------------------------------------------------

The pizza party example and the suggested habits extend to a more general principle for a remote-first culture: **we should use online tools so everyone can participate equally in the work we do.**

When people work in the same space, some of the context of how work gets done is immediately accessible. We can see a colleague getting frustrated, or two people discussing a complex piece of work. When people are working remotely, these cues aren't there anymore. We generally see the artifacts produced by that work - the output - but not the context of how those artifacts were created. Some of the online tools we use, like videoconferencing and chat, are oriented towards immediate interactions and help transmit the context of work throughout a distributed team.

If you've ever tried to find something from six months ago in a chat history, though, we know that something more is needed. One of the people mentioned that their organization actually requires people in videoconference meetings to transcribe the decisions into a system of record during the meeting, which can help make sure they are properly captured and that people agree with the way they're written. The importance of handoff records across time zones was also mentioned. These are examples of another useful principle: **conclusions must go through a source of truth.** One organization even goes so far as to delete chat histories after 7 days, helping ensure they don't base work on things that aren't shared where other people can learn about the direction.

We actually face issues with making our work visible even when everyone is working in the same location; a remote-first culture makes it more important that we make our processes and work visible. As one person put it, we need to have visible output - otherwise, people assume you're doing nothing.

For developers, a potentially useful technique is to have a channel where people post links to their merge requests when they open them; team members can react with 👀 to indicate that they're looking at it, helping with coordination in the team. Another suggestion was to make sure you're opening work-in-progress merge requests so that teammates can see what you're working on and the progress you're making. [Note: If, however, you're working on short-lived branches (<1 day), you may be better off just opening the merge requests.]

One person mentioned a technique they use as a remote individual, which is to install software on their computer that automatically tracks the time they spend online working. Something to consider before heading down this path, though, is whether that's actually helping make your work visible to other people; it may just be pulling us towards activity rather than the actual achievement of outcomes.

Managing distributed teams
--------------------------------------------------------------------------------

The question of time tracking raises a basic management question: what is expected when working remotely? In a corporate setting, how you answer this question this will interact with (and needs to support) the assessment and performance management processes.

When remote people are first introduced to a team, managers also need to be ready to address questions from existing team members. A useful question to ask is "why do we want _this_ person?" even though they're not co-located with the rest of the team. Knowing the answer to it can help people adjust to the changes needed for remote work to be effective.

Communication is central to any team's success, but with distributed teams we need to be more intentional about it. In contrast to conventional co-located teams, conversations among remote colleagues don't happen when people are walking to get coffee. Communication needs to be proactive, and should be among our expectations for all team members. Ideally, part of this is communication occurs in real time. A useful technique is to have a couple of hours of overlap. If you're all in the same time zone, still have everyone call in for the daily standup.

Ultimately, we want to build relationships with people that drive and own value delivery; _trust_ is a central piece of remote-first culture allowing these relationships to thrive.

---

**_Thank you to everyone who participated in this discussion; the experiences and insights you contributed are appreciated._**

---

Since the conference, I finished reading Camille Fournier's _The Manager's Path_. In the final chapter, _Bootstrapping Culture_, she writes:

> In complex environments where the needs of the group must override the need of the individual, cultural values are the glue that enables us to work as a team and make decisions when faced with uncertainty. This is why figuring out and guiding your culture is such an important part of building a successful company. (Fournier 2017, p. 199)

Reading this reinforced what is perhaps my top takeaway from the discussion: working successfully as a distributed team is fundamentally a question of culture, and we are all, each and every one of us, responsible for shaping it through our daily habits.

---

References
--------------------------------------------------------------------------------

Fournier, Camille. 2017. _The Manager's Path: A Guide for Tech Leaders Navigating Growth & Change_. Sebastopol, CA: O'Reilly.
