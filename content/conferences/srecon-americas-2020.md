---
title: "SREcon Americas 2020"
date: 2020-12-07
summary: >
  December 7-9, 2020 — Virtual
---

December 7-9, 2020 — Virtual

The talks:

* [Robert Barron — Failure is Not an Option! SRE Lessons 50 Years after the Apollo 13 Flight to the Moon](#barron)
* [Daria Barteneva — Study on Human Factors and Team Culture to Improve Pager Fatigue](#bareneva)
* [John Blaho — A Bartender's Guide to Network Monitoring](#blaho)
* [Prathyusha Charagondla — The Good, the Bad and the Ugly: The 3 Learnings of an SRE](#charagondla)
* [Danny Chen — Capacity Planning and Performance Enhancement with Page Reference Sampling](#chen)
* [Morgan Collins — Incident Response in Unfamiliar Sociotechnical Systems: One Incident Commander's Challenges Supporting Inter-organizational Anomaly Response in the Age of COVID-19](#collins)
* [Alex Elman — Are We Getting Better Yet? Progress Toward Safer Operations](#elman)
* [Liz Fong-Jones — Identifying Hidden Dependencies](#fong-jones)
* [Kyle Guichard and Venus So — Soft Failures, Hard Goals - Accelerating Payments at Scale During the Pandemic](#guichard-so)
* [Mark Hahn & Thomas Hahn — Achieving Mutual TLS: Secure Pod-to-Pod Communication Without the Hassle](#hahn-hahn)
* [André Henry — It's a Trap! How Abstractions Have Failed Us.](#henry)
* [Nora Jones; Fred Hebert; Lorin Hochstein; Vanessa Huerta Granda — Learning from Adaptations to Coronavirus](#jones-hebert-hochstein-huerta-granda)
* [Markus A. Kuppe — Weeks of Debugging Can Save You Hours of TLA+](#kuppe)
* [Tom Limoncelli — Low Context DevOps: Improving SRE Team Culture through Defaults, Documentation, and Discipline](#limoncelli)
* [Laura Maguire, PhD — The Secret Lives of SREs - Controlling the Costs of Coordination across Remote Teams](#maguire)
* [Anika Mukherji — Building Actionable Code Ownership](#mukherji)
* [Alex Nauda — Production Population Control: My Cattle are Rabbits!](#nauda)
* [Mikolaj Pawlikowski — Why SREs can't afford to NOT do Chaos Engineering](#pawlikowski)
* [J. Paul Reed — When /bin/sh Attacks: Revisiting "Automate All the Things"](#reed)
* [Nishant Roy — Heap Optimization for Go Systems](#roy)
* [Raj Shekhar and Mehmet Can Kurt — Hot Swap Your Datastore: A Practical Approach and Lessons Learned](#shekhar-can-kurt)
* [Daniel "Spoons" Spoonhower — Building Service Ownership Using Documentation, Telemetry, and a Chance to Make Things Better](#spoonhower)
* [Cory Watson — Observing from Incidents](#watson)
* [James Wickett — Pragmatic Security for SRE](#wickett)
* [Christina Yakomin — Cloudy with a Chance of Chaos](#yakomin)
* [Moshe Zadka — Jupyter as Incident Response Tool](#zadka)


# Day 1: Monday 2020-12-07

## <a name="maguire"></a> The Secret Lives of SREs - Controlling the Costs of Coordination across Remote Teams

[Laura Maguire, PhD](https://twitter.com/LauraMDMaguire)

**Twitter threads:**
[cornazano (me)](https://twitter.com/cornazano/status/1335965290035884033)
| [richburroughs (Rich Burroughs)](https://twitter.com/richburroughs/status/1335965242107424769)

**My livetweet contents**

> First talk of the day is @LauraMDMaguire, talking about Adaptive Choreography. #SREcon

> Keeping highly reliable systems (911, health records, transportation, entertainment, ...) well maintained, better, and faster takes considerable effort. Her research work focused on this work and the people who perform it. #SREcon

> The pandemic made a lot of our dependency on technology visible to people. Moved from people not being interested, to "have you finished that research yet?" #SREcon

> We stretch the capabilities of the tech, and the capabilities, skills, and capacity of the people who keep these systems running. #SREcon

> There is resilience and adaptive capacity in the people doing the work, despite the organizational processes that don't always help us in time-pressured situations.
>
> Cognitive work and detailed efforts of being an SRE is hidden. Going to focus on it. #SREcon

> Taking a cognitive systems view of working in complex systems to see how we can learn and support people.
>
> Risk is largely emergent, successful performance requires adjusting rapidly to changing conditions. #SREcon

>How do we define expert performance in conditions of uncertainty?
>
>There's always more to the story when something goes wrong. #SREcon

> How do responders manage the work, when we also need to coordinate among people since everyone's mental model of the system is different and partial? These circumstances increase cognitive load. #SREcon

> Shared rooms vs. remote: remote adds complexity as we lose the implicit context present in a shared location. #SREcon

> Tradeoff decisions made at points in the past have consequences during the time-pressure of an incident, and produce additional cognitive demands.
>
> Communication/coordination demands also escalate, but they're hard to see. #SREcon

> Understanding dynamics during operational incidents can help guide design for how we coordinate. How someone looks at a problem can make a difference - who to contact, when? sufficient expertise, context for impacts? #SREcon

> When context is held in head, we are able to be really efficient at response. 
>
> Needs knowledge about the system, the team, the organization, and about "others" (users, vendors, etc.). #SREcon

> This knowledge the foundation for proactive actions during an incident; the more that it is shared, the more easily we establish common ground during a problem. #SREcon

> Incident response is not a linear activity that occurs in discrete phases. There is a lot of uncertainty, interruptions, coordination. We have overlapping and concurrent demands. #SREcon

> The incident command role can surpass the capability of the person filling it; that is a bottleneck in the speed of incident response. Can we distribute the coordination instead of centralizing it? #SREcon

> Multiple responders all responsible for coordination in this type of system. We already likely do this: "I'm checking the logs" is the taking of initiative (not a delegated assignment from the incident commander). #SREcon

> Expert practitioners use small utterances that are *not* understood easily by outsiders. They do establish common ground, at speed, among the practitioners.
>
> [That compressed communication reminds me a lot of studying mathematics, science, linguistics, etc.]
>
> #SREcon

> Expert practitioners, working together, are able to detect lack of understanding, and quickly coordinate to re-establish common ground.
> 
> It is ultimately up to the industry to support engineers who maintain these systems that are critical to our society. [fin]
>
> #SREcon


## <a name="fong-jones"></a> Identifying Hidden Dependencies

[Liz Fong-Jones](https://twitter.com/lizthegrey) (Honeycomb)

**Twitter threads:**
[cornazano (me)](https://twitter.com/cornazano/status/1335977536573104130)
| [richburroughs (Rich Burroughs)](https://twitter.com/richburroughs/status/1335977484223873025)

**My livetweet contents**

> Second talk of the day is @lizthegrey talking about Identifying Hidden Dependencies. #SREcon

> Honeycomb deploys over a dozen times per day (including Fridays). Requires investment not only in continuous delivery, but continuity of operations. #SREcon

> Stateful services are scary to operate, especially if we're only familiar with stateless services. Data and stateless services are operationally challenging. Needed to quantify reliability in this context. #SREcon

> SLOs establish a reliability constraint. We don't need them to be 100% available and reliable - and can't be in a distributed world. #SREcon

> With a stateful service, the success of storing data is important and becomes one of the things we need to measure. Queries also have SLOs. When we're exceeding the SLOs, we can [and should!] invest in improving via injection of chaos in the system. #SREcon

> A data pipeline is crucial if you've already committed to ingesting customer data, but have not yet persisted it. We really don't want this type of pipeline to fail! #SREcon

> Portions of these types of pipelines don't change frequently. This produces hidden risks, since we don't test the redundancy processes regularly. With data, this needs to include integrity and consistency. #SREcon

> A lot of the failover scenarios that are designed are great in theory - but how do we know if they work?
>
> [Thinking about @LauraMDMaguire's story about backups during her talk.]
>
> #SREcon

> This is where we can engage in chaos engineering - controlled experiments in meaningful environments. We need to be able to control the scope of impact, abort the experiment, and observe and diagnose what happens. #SREcon

> Before running the experiment, make sure that it has a hypothesis. We don't want to just inject chaos into our systems. #SREcon
>
> ❤️

> Performing experiments on clean restarts allowed for issues to be detected and resolved while people were in their normal working hours, rather than dealing with impaired redundancy overnight. #SREcon

> These experiments help with de-risking our systems, reducing their fragility. They also provide information that feeds back to our design efforts. #SREcon

> Once one-off tests were succeeding, started performing continuous verification of the reliability investments. Doing restarts every Monday helps avoid unintended regressions. #SREcon

> This also helps determine where spot instances can be used without impacting durability of data - saving $ on AWS bills. #SREcon

> "There's no such thing as a failed chaos experiment."
> 
> Celebrate "success" since it means your system works. Celebrate "failure" because you learned about things you need to fix.
>
> #SREcon


## <a name="elman"></a> Are We Getting Better Yet? Progress Toward Safer Operations

[Alex Elman](https://twitter.com/_pkill) (Indeed)

**Twitter threads:**
[cornazano (me)](https://twitter.com/cornazano/status/1335992137368875010)
| [richburroughs (Rich Burroughs)](https://twitter.com/richburroughs/status/1335986372847443974)

**My livetweet contents**

> Next up: @_pkill discussing our progress towards safer operations. #SREcon

> Success is the driver of more complexity; this is the *law of stretched systems*. Capacities being stretched by organizational workload, development pace, expertise, innovation. #SREcon

> Contrast two safety modes: "learn and adapt" versus "prevent and fix". We may prioritize one or the other in an organization.
>
> Learn and adapt enables prevention and repair, but is better in that it produces greater safety over time.
>
> #SREcon

> How do we measure progress? 
>
> "It is wrong to suppose that if you can't measure it you can't manage it." - Deming
> 
> #SREcon

> Distinguishing between being data-driven and being driven by data. Data isn't the only way to make decisions. #SREcon

> If you pair metrics with the wrong story, you arrive at the wrong conclusion. Stories are what give meaning to the metrics. #SREcon

> We don't need to wait for incidents in order to get better. We can engage in chaos engineering. This is a learn and adapt strategy that won't really be valued in a prevent and fix world. #SREcon

> Incident report give us hindsight that the incident responders didn't have access to. Comparing incidents to escape rooms: analogues, but production has higher consequences than the escape room. #SREcon

> We need to figure out how to enhance human capabilities and performance, not how to prevent people from the system (guardrails). #SREcon

> This! --> "Incidents are a source of insights but not a good measure of reliability." #SREcon

> Control is the ability to impose our will over production systems; we can't really get this.
>
> Influence is the ability to modify context/inputs to improve our chances of getting to a good outcome.
>
> #SREcon

> Opportunities are taken, not given. We can evaluate whether the goals are right, and select among them, and make choices. #SREcon

> Discussing Gary Klein's work. To increase performance, we need to both decrease errors *and* generate insights. Having only the first of those doesn't make the amount of difference we want. #SREcon

> Prevent-and-fix establishes a focus on local-only fixes, that are below the line of representation - purely tech - but we need the wide view over how the work gets done above the line. That's where we have leverage to make a difference. #SREcon

> What are we looking for in incident analysis?
>
> We can learn about exchanges - which items are information seeking, information providing, mitigation proposals, actions taken/not taken?
>
> [This sounds similar to several discourse analysis techniques in linguistics.]
>
> #SREcon

> A single table of events and phases of the incident appears authoritative, promotes one perspective over others. We can consider, instead, a timeline that combines them with the parallel activities of the responders; incident writeups privilege multiple perspectives. #SREcon

> Interviews can elicit tacit knowledge that is important to understanding; the questions we ask can facilitate getting this information. #SREcon


## <a name="watson"></a> Observing from Incidents

[Cory Watson](https://twitter.com/gphat)

**Twitter threads:**

[richburroughs (Rich Burroughs)](https://twitter.com/richburroughs/status/1336020801066156032)


## <a name="spoonhower"></a> Building Service Ownership Using Documentation, Telemetry, and a Chance to Make Things Better

[Daniel "Spoons" Spoonhower (Lightstep)](https://twitter.com/save_spoons) (Lightstep)

**Twitter threads:**
[cornazano (me)](https://twitter.com/cornazano/status/1336021207641100288)

**My livetweet contents**

> Next talk: @save_spoons, talking about building service ownership. #SREcon

> SRE teams are now navigating multiple dev teams. In a sense, SREs now need to scale themselves. #SREcon

> Once we split up our systems, we need to figure out how it aligns to the organization in terms of responsibility. 
>
> Service ownership has to do with responsibility for both software and service, hopefully leading to higher rates of delivery. #SREcon

> Ownership is, fundamentally, about accountability and agency. If we're going to have smaller SRE teams with software teams owning the service, it requires documentation, oncall processes, and telemetry. #SREcon

> Distributed tracing involves spans - events that describe work done by a service - and traces - a collection of spans associated with a request sent to our system. This orients us towards the client's experience. #SREcon

> When we look at distributed tracing: traces are the structured event record, tracing is the process of deriving value from that information.
>
> Tooling for this is evolving; look at #opentelemetry for more on this.
>
> #SREcon

> Centralized documentation is about discoverability of things like: experts, telemetry, and playbooks. These should have standard formats to keep consumption relatively fast. #SREcon

> If the documentation is machine readable, we can go further and consume and make updating it part of the regular work rather than a separate thing to maintain. The updates are a side effect of the work, rather than supplemental effort. #SREcon

> Neat thing about distributed tracing - it can automate the discovery inter-service dependencies! #SREcon

> Oncall differs from other work in that it is more akin to a performance than most other work we do. Documentation can help with building confidence in preparation for that performance. #SREcon

> Moving towards ownership can be done iteratively. As we get signals showing that we need to split operational work, we can mitigate the stresses of it. Example: include experts in the rotation, balance number of services to learn. #SREcon

> Useful thing to do: link to evidence of the problem, including the traces that allow you to navigate up and down the stack. This helps make information more visible, instead of just being in people's heads - and speeds up mitigation. #SREcon

> [Interesting thing to think about: linking the traces this way can help with initial establishment of common ground among responders.] #SREcon

> Postmortems are part of the process - and they are documentation! 
>
> As documentation, centralization and standardized structure are useful. #SREcon

> The reasons that oncall is important is part of why _improving_ oncall is also important. We need to be able to communicate this to management. [@marcocoulter's discussion of negotiaton from earlier today becomes relevant here.] #SREcon

> Internal SLOs within a system of services should be derived from the client-facing SLOs; distributed tracing can help us with this derivation.
>
> [Related idea in lean is to start improvements at the pacemaker process at the boundary with the client.]
>
> #SREcon

> If we want to move to a service ownership model, documentation, oncall, and SLOs are the key pieces to the puzzle of how we get there.
>
> Making it part of the day-to-day work serves as a ramp to getting there. #SREcon


## <a name="bareneva"></a> Study on Human Factors and Team Culture to Improve Pager Fatigue

[Daria Barteneva](https://twitter.com/DashaRV) (Microsoft)

**Twitter threads:**
[cornazano (me)](https://twitter.com/cornazano/status/1336032111690731520)
| [richburroughs (Rich Burroughs)](https://twitter.com/richburroughs/status/1336032016400142336)

**My livetweet contents**

> Next talk: @DashaRV talking about human factors and pager fatigue. #SREcon

> Oncall involves intentionally unpredictable work. We're not alone - other professions like medicine and firefighting are also dealing with this type of demand-driven work. #SREcon

> "It's just work, nothing you can do" was the general attitude about oncall several years back. But if it's bad, it's likely a symptom - and we can learn to do better. #SREcon

> Today, we more often discuss psychological safety and empathy. These impact team happiness and dynamics. #SREcon

> Blameless culture is part of this. Make sure that we acknowledge that learning is important, and is a form of success. This can't happen if people fear negative reprecussions. #SREcon

> Leadership needs to allow time for team members to develop technical literacy and expertise on the systems. This also needs to include documentation to capture what we've learned for the *future*. #SREcon

> Structured and unstructured meetings enable different team dynamics, and can help us do things better through a mix of the two. #SREcon

> Building feedback loops is needed. Example: a survey report that is never read doesn't change anything. #SREcon

> And where this isn't working well, remember... each of us is a change agent, and we can take action to make a difference! #SREcon


## <a name="mukherji"></a> Building Actionable Code Ownership

Anika Mukherji (Pinterest)

**Twitter threads:**

[cornazano (me)](https://twitter.com/cornazano/status/1336039645898027012)
| [richburroughs (Rich Burroughs)](https://twitter.com/richburroughs/status/1336038131192057856)

**My livetweet contents**

> Not doing a full liveweet of Anika Mukherji talk, but really like the question of "do we want ownership of lines of code, or ownership of functionality?" #SREcon


## <a name="zadka"></a> Jupyter as Incident Response Tool

[Moshe Zadka](https://twitter.com/moshezadka) (Twisted Matrix Laboratories)

**Twitter threads:**
[cornazano (me)](https://twitter.com/cornazano/status/1336044477346144269)

**My livetweet contents**

> Last talk of the day is @moshezadka, helping us understand how we can use Jupyter as part of our incident management tooling. #SREcon

> Jupyter started as a data-science tool, supporting exploration in shared environments, with the ability to execute code. The sharing and exploration is also fairly central to resolving incidents. #SREcon

> We can collect screen snapshots, and query data via Python, all within the Jupyter notebook. This analysis may be easier than constructing the same information in monitoring-specific tooling (e.g., Prometheus). #SREcon

> The queries and analyses can all be in individual cells in the notebook, which can be re-executed as we proceed through the incident. #SREcon

> Since the notebook can be persisted and shared, we can use it as part of our preparation for the retrospective on the incident. Idea: we have most of the notes already captured inside the notebook. #SREcon

> We can extend it with additional text, adding cells as needed for the notes about what we were seeing/thinking at the time. And then... export it to HTML so that others can read the report without needing Jupyter running. #SREcon


## <a name=""></a> Sustainable Software Engineering & SREs

[Bill Johnson](https://twitter.com/dubrie) (Microsoft)

**Twitter threads:**

[richburroughs (Rich Burroughs)](https://twitter.com/richburroughs/status/1336043924163465217)


# Day 2: Tuesday 2020-12-08


## <a name="reed"></a> When /bin/sh Attacks: Revisiting "Automate All the Things"

[J. Paul Reed](https://twitter.com/jpaulreed) (Netflix)

**Twitter threads:**
[cornazano (me)](https://twitter.com/cornazano/status/1336325226020229121)
| [richburroughs (Rich Burroughs)](https://twitter.com/richburroughs/status/1336325149574852614)

**My livetweet contents**

> First talk of the day today is one I'm really looking forward to - @jpaulreed revisiting the mantra of automate all the things! #SREcon

> Going to be looking at how to make automation a better partner. This is useful if we're an old hat at bash, or newly entering the automation game. #SREcon

> Frequently, "automated" things involve scripts, runbooks, monitoring, forked scripts and runbooks that aren't updated and diverge - and we drift into issues. #SREcon

> Boeing 737 max is an example of a long drift into failure, exemplifying the types of perils with automation that occur with long-running systems. #SREcon

> The Knight Capital incident shows us how quickly automation can change our world.
>
> [And the slide counting up of financial loss is beautiful for discussing this example.]
>
> #SREcon

> When we say automation, what do we mean? Maybe it's shell scripts? #SREcon

> One way of thinking about it is as a spectrum: runbooks <-- script -- orchestration --> ml/ai.
>
> We also have layers of automation as we move through the our delivery pipelines.
>
> So there are multiple axes of spectrums to consider. 
>
> #SREcon

> Hooking up our tools to one another generates a complex set of interactions that we depend on and interact with on a daily basis. #SREcon

> Consideration of issues goes back to at least Banbridge's Ironies of Automation paper (1983).
>
> [I like this paper, glad to see a reference to it here!]
>
> #SREcon

> Ironies:
>
> * Manual skills deteriorate when not used.
>
> * Generation of new strategies requires adequate knowledge of systems.
>
> * Usage of automation may depend on operators skills that were developed before the automation was implemented.
>
> #SREcon

> * There is a speed vs correctness tradeoff involved; how much tolerance do we have for loss of correctness?
>
> * Automation can camouflage current system state, leaving us without context.
>
> #SREcon

> * Understanding the current state, and tracing how the system got there, are difficult. 
>
> * Can you sit here and monitor this fully automated system to make sure it's doing it's job correctly?
>
> #SREcon

> Frequently, automation isn't valued and is treated as disconnected from the application that it is automating. #SREcon

> Introducing Joint Cognitive Systems. Key capabilities among agents in the system: autonomy, authority, directed attention, redirectability, and interpredictability.
>
> The last three are not generally present in the automation, but are fundamental for coordination.
>
> #SREcon

> We can look at automated systems either as a deterministic machine (in hindsight) or as an agent acting independent of the operator (in context). #SREcon

> Looking at the Rasmussen Triange now - which establishes constraints on what we do.
>
> We move away from two of these boundaries, putting pressures on the system:
>
> * Cheaper, better, faster.
> * Maximum work, minimum effort.
>
> #SREcon

> These push us towards the third boundary, and when we cross it things go *boom*; there is a discretionary space before we cross that boundary, but automation is brittle here; we need humans to navigate near the edge of that space. #SREcon

> Checklists can be used as a collaborative tool; when two people use it together, you can get a lot of additional observations. This can help with learning about the sharp edges before we automate an activity. #SREcon

> There are practices to help operators cope with the ironies. Simulation, widening our system understanding [learning reviews are great here], checks > locks lets operators deal with more situations. #SREcon

> The amount of time pressure that will affect people using the automation should be taken into account when designing it. #SREcon

> For those capabilities that automation isn't good at, we can consider restricting the scope and factoring the automation design so that it works with the operators. #SREcon

> "Automation isn't (usually) dangerous, but the way our industry thinks about it can be."
>
> #SREcon

> We need to treat automation as a product, and we need to make progress on building it in ways that integrates into our operational joint cognitive systems. #SREcon


## <a name="pawlikowski"></a> Why SREs can't afford to NOT do Chaos Engineering

[Mikolaj Pawlikowski](https://twitter.com/mikopawlikowski) (Bloomberg)

**Twitter threads:**
[cornazano (me)](https://twitter.com/cornazano/status/1336336370546008066)
| [richburroughs (Rich Burroughs)](https://twitter.com/richburroughs/status/1336336241457942529)

**My livetweet contents**

> Next up: @mikopawlikowski discussing chaos engineering and why SREs can't afford to not do it. #SREcon

> Chaos Engineering (CE) is, at the core, about experimenting on a system to build confidence to withstand turbulent conditions - like those our services experience in prod. #SREcon

> What we really care about is reliability [in the face of those turbulent conditions]. #SREcon

> There's an overlap between SRE and CE - we may even view CE as a subset of SRE. #SREcon

> Myths about CE:
>
> * it's just chaos monkey
> * it's just testing in prod
> * it's only for distributed systems
> * it only works on tech X
> * it's just breaking things randomly
>
> None of these are correct. #SREcon

> Important point: don't necessarily start CE in production; we can start experimenting in other less critical environments! #SREcon

> Once you get a good understanding of your system, you can design a tightly-controlled experiment to find out how the behaves under specific conditions. #SREcon

> Four steps needed for CE:
>
> 1. Observability - we need to be able to measure some variable
>
> 2. Steady state - what does the range of the variable typically look like?
>
> 3. Hypothesis - predict what will happen when X occurs
>
> 4. Run the experiment!
>
> #SREcon

> [He's running some demo experiments here, showing off what chaos experiments look like.] #SREcon

> To get buy in: need to have a conversation about risk and rewards with management.
>
>People overestimate some low probability risks (ex: risk of getting attacked by shark, but heart disease is a lot more likely as a cause of death). #SREcon

> This is also good for our teams. CE helps us get woken up less often, and can help improve our team's resilience (example: have someone be slow or unavailable during a specific experiment). #SREcon


## <a name="collins"></a> Incident Response in Unfamiliar Sociotechnical Systems: One Incident Commander's Challenges Supporting Inter-organizational Anomaly Response in the Age of COVID-19

Morgan Collins (Salesforce)

**Twitter threads:**
[cornazano (me)](https://twitter.com/cornazano/status/1336347911274311683)
| [richburroughs (Rich Burroughs)](https://twitter.com/richburroughs/status/1336346635903758338)

**My livetweet contents**

> Next up is Morgan Collins, talking about incident response in unfamiliar sociotechnical systems - and some of the challenges faced during a pandemic. #SREcon

> Starting with an overview of the Incident Command System (ICS) and how it was created in the 1960s. One description is in terms of a reporting/managerial reporting, but that's not the interesting description of it... #SREcon

> 1960s saw increasing # of wildfires in California. This exposed coordination challenges across the disparate organization structures. This lead to a lack of interpredictability. #SREcon

> FIRESCOPE was a precursor to ICS, seeking better communications and resource management during these wildfire incidents.
>
> Needed to also be flexible, repeatable, and inexpensive. This allowed development of expertise.
>
> #SREcon

> ICS id delegation driven, defining roles and reporting chains. At the top of this structure is the incident commander, who is the centralized leader for managing the incident. #SREcon

> Mid-1980s saw increasing adoption of ICS nationally and internationally. Following 9/11, it has evolved into NIMS (National Incident Management System). #SREcon

> If you're working within the NIMS framework, it helps ensure that you have compatible systems for mutual support during incidents. #SREcon

> ICS has seen some success in private enterprise for dealing with operational incidents. The repeatability is useful, and it helps establish common ground via shared terminology, pre-defined signals and conditions under which we act. #SREcon

> ICS is frequently adapted for private enterprise. The model is often scaled down (fewer roles); cost is less emphasized; generally have static resource pools with expertise brought in dynamically as needed; and mutual aid is often *not* a goal. #SREcon

> With this, coordination across teams isn't emphasized and we have more issues with establishing common ground when we do need to do this. #SREcon

> With COVID-19, we get a spike on service [hello, increasing # of wildfires...]. Customer patience is lower as we have critical systems under these pressures. And we're adjusting by bringing more people into the incident response process. #SREcon

> The "warm blanket" fallacy: Bringing in an experienced incident commander will guarantee flawless execution in unfamiliar environments.
>
> Reality: it will not.
>
> #SREcon

> If you're asked to step in because we need an incident commander *now*, we encounter challenges with conventions / roles in the specific team. For example: who handles public communications?
>
> This undermines our mental models of what we are supposed to be doing. #SREcon

> Recommendation when using a video bridge: Insist on webcams. It can help compensate for the loss of signals we have with in-person work. #SREcon

> A necessary part this is to nurture the establishment of common ground. This needs to be balanced to not interfere with critical work - ask "when will we update this" rather than constantly asking "are we done?" #SREcon

> Short and missing answers to questions are signals that common ground is at risk. #SREcon

> We should be working on decentralizing command; the incident commander needs to avoid becoming a bottleneck within the response efforts. #SREcon

> After the end of an incident, it's useful to talk right afterwards. It allows comparison of mental models - but there's a tradeoff. It can help with building the ability to respond as a team going forward, but can impede later incident analysis. #SREcon

> This also gives opportunities to discuss ephemeral things that will be forgotten later: cues people were reacting to, observations about what others did well. #SREcon


## <a name="limoncelli"></a> Low Context DevOps: Improving SRE Team Culture through Defaults, Documentation, and Discipline

[Tom Limoncelli](https://twitter.com/yesthattom) (STack Overflow)

**Twitter threads:**
[cornazano (me)](https://twitter.com/cornazano/status/1336358927861231618)

**My livetweet contents**

> Last talk of the morning: @yesthattom discussing low context devops! #SREcon

> Using low-context techniques can help our teams work more effectvely.
>
> Can we get to a point where people are not blocked waiting for someone else with expertise?
>
> Can we get to a point where one person learning something converts to the entire team learning it?
>
> #SREcon

> Story: Person arrives in village, tries to talk to shopkeeps but they refuse. Eventually, a little boy tells him he needs to talk to the village elders first. The visitor does, and then he can buy things.
>
> Perspectives: How can he learn this? vs How could he not know? #SREcon

> A high context culture: communication is implicit; relies on long term relationships.
>
> A low context culture: communication is explicit, rules are known, codified.
>
> #SREcon

> Low context is important for environments that people don't spend much time - airports, for example. #SREcon

> There's a sign in Penn Station that is only interpretable to someone who knows a 30-year history of the station, since it uses a station name that changed that long ago.
>
> Someone has been changing the lightbulb in that sign for the past 30 years. #SREcon

> Part of this is that we need to make it easy to do things right. 
>
> "We want to set up our coworkers so that they fall into a pit of success." 
> 😂
>
> #SREcon

> Another element we should pursue is ubiquitous documentation. Example: taxi lines that guide us. It is available when and where you need it. #SREcon

> We can pursue this in our development contexts, providing links at the right place and time - when people are in context of a process, include a relevant link. #SREcon

> For this to work well, we need to create a culture that updates doc as we work. The doc needs to be treated as important - file bugs, allocate time, update as we go. #SREcon

> "I like having written a book, I don't like writing a book."
>
> Why do people dislike writing documentation?
>
> 1. uncertain scope - what's needed?
> 2. uncertain audience - who's reading it?
> 3. blank screen - where do I start?
>
> #SREcon

> Templates can help mitigate some of this (especially the blank screen). Service doc and alert doc templates also help shape our understanding of the scope and audience. #SREcon

> We need to include documentation in our work estimates - and write it in small batches, updating it as we go.
>
> Another tip - pull information from the places they already write: email, chat, etc. Ask them if they can copy it to the doc repo!
>
> #SREcon

> Who makes changes happen in our organizations? We do.
>
> This is a difference between *leadership* and *management*. Management is a role, leadership is a behavior - going first and making it easier for others to follow. We make these changes happen by leading.
>
> #SREcon

> We should strive towards low-context environments. Paths to help us get there:
>
> * Smart defaults
> * Make right easy
> * Ubiquitous documentation
>
> #SREcon


## <a name="yakomin"></a> Cloudy with a Chance of Chaos

[Christina Yakomin](https://twitter.com/SREChristina) (Vanguard)

**Twitter threads:**
[cornazano (me)](https://twitter.com/cornazano/status/1336376881269022720)
| [richburroughs (Rich Burroughs)](https://twitter.com/richburroughs/status/1336377000961822720)

**My livetweet contents**

> First talk of the afternoon is @SREChristina, "Cloudy with a Chance of Chaos". #SREcon

> Chaos engineering (CE) involves fault injection, but "breaking things on purpose" is an oversimplification.
>
> "Isn't that a fancy name for performance testing?" Well, it includes that, but load isn't the only type of fault.
>
> #SREcon

> A short, catchy version: chaos engineering = resilience testing. 
>
> [Also shared the same reference definition that @mikopawlikowski cited earlier today.]
>
> #SREcon

> When we start digging into how to identify experiments, we can start with the architecture diagrams and do a failure modes and effects analysis. #SREcon

> Graceful degradation - if a recommendations service is failing, pages in a shopping site should still render. To test this, we can run a chaos experiment where we inject failures into the system. #SREcon

> If the database storing reviews is unavailable - how do we want the system to behave? What is our *expectation* of the client's experience? Once we know that, we can run an experiment to test that, too. #SREcon

> Why is it valuable? We're getting more comfortable using commodity compute resources - treating our servers as cattle. During an incident is not the time we want to discover that our resilience mechanisms don't work as intended. #SREcon

> CE experiments for things where the [technical] system isn't resilient can help our teams, training people to respond effectively during incidents. #SREcon

> For Vanguard's specific use case, the open source tools presupposed some types of accesses that couldn't be allowed. Since they didn't yet have buy-in to committing purchasing a vendor solution, they started building the ability to inject certain types of faults. #SREcon

> They built this in alignment with four guiding principles. #SREcon

> First guiding principle: serverless architecture.
>
> High availability was important, as was cost. They wanted to make sure there was no significant cost when experiments weren't running. #SREcon

> As part of this, they've reduced the technical footprint of their system - using Python (same language as the system), reducing the number of frameworks and languages that people need to switch among. #SREcon

> Demand is sporadic. The serverless approach made a difference between hundreds of dollars per month and tens of dollars per month. #SREcon

> The platform they've built supports both ad-hoc and scheduled experiments, letting people run the experiments on a recurring basis. #SREcon

> Second guiding principle: Easy adoption.
>
> Teams can self-serve access the tool; engineered to avoid needing code changes - may be as little as a tag added to resources in AWS; and the tool is well documented.
>
> #SREcon

> Third guiding principle: Defined guardrails.
>
> Since all IT has access to the tool, they need a way to manage this - prioritizing single-target experiments, using tags to control opt-in to experiments, start with non-production while proving the approach. #SREcon

> Fourth guiding principle: Integrated reporting.
>
> Fault injection is pointless if you can't see the results. They have steady state probes before running the experiment as part of this, and the tool provides common visualizations. #SREcon

> This provides the bare minimum needed to start running experiments; the expectation is that some teams will have better tooling, adapted to their specific context - but this keeps teams from being left behind. #SREcon

> Among the future steps for their team, considering whether there is a way to run CE experiments with every change. #SREcon


## <a name="wickett"></a> Pragmatic Security for SRE

[James Wickett](https://twitter.com/wickett) (Verica)

**Twitter threads:**
[cornazano (me)](https://twitter.com/cornazano/status/1336387724308262912)
| [richburroughs (Rich Burroughs)](https://twitter.com/richburroughs/status/1336388055343661056)

**My livetweet contents**

> Next up is another one of the talks I've been looking forward to today: @wickett, "Pragmatic Security for SRE".
>
> #SREcon

> We spend a lot of money and time on security, but something's amiss - we're often protecting the wrong things, and hurting productivity in the process. #SREcon

> Fallacy: if we add in risk management, we can do less in the code. But... we've continued to reduce investment in security engineering, and we're seeing the results of this. #SREcon

> Security tends, in isolation, to be opposed to change. (This rhymes with the situation with operations over the years.) #SREcon

> What happened to bring ops into the process of delivering value? We need to extend this to the security folks.
>
> DevSecOps is about bringing security out of their silos and bring it into the pipelines.
>
> #SREcon

> There are reliability and security tradeoffs. Example: higher redundancy has more attack surface. #SREcon

> Looking into the State of DevOps results about high performing teams. They aren't introducing new types of tools; rather, they're shifting it left in the pipeline. #SREcon

> Instead of treating security as a stage late in the pipeline, we can integrate security concerns into each of the phases of the pipeline: develop, inherit, build, deploy, operate. #SREcon

> During development, we can consider things like threat modeling, security stories, security tests in the unit testing stage. #SREcon

> As part of our development standards, we can include pre-commit hooks related to security. We can also bring usual development tooling (linting, reviews, etc.) to our security teams. #SREcon

> Security bugs are not a special class of vulnerability. We should do security testing in the same places where other error testing lives.
>
> Security bugs are mistakes in code that are exploitable - and we can't know until much later (maybe even not until it's exploited). #SREcon

> Some useful questions: Are developers testing for security locally? Are we preventing secrets from leaking into the pipeline? #SREcon

> The inheritance phase is about dependencies. Your real LOC count includes everything in every framework and library you depend on, and even the OS below it. We need to think about the supply chain from a security standpoint! #SREcon

> The build phase is often considered the "core" of CI. Here, we can run security scans on the running application, security configurations, and the like. We also want to probe for security issues at this point. #SREcon

> Some useful questions: Am I testing for low hanging security fruit? Am I running attack tools to exercise my application? #SREcon

> During the deploy phase, we're looking at compliance, audit, authorization, and logging. We want to get to a point where deploys are just standard changes, and bring auditors along on the journey. #SREcon

> Useful questions here: What secrets do we need to deploy? Is it a repeatable mechanism? Do we verify compliance on every deploy? #SREcon

> Security in the operate phase needs to feed back to the developers. We need to detect things that matter - areas of our site that are under attack, vectors being exploited in the wild - and that needs to inform our investments. #SREcon

> Our systems are now too large for us to hold in our heads. Security chaos engineering can help with this - targeted CE experiments where the injected fault is a security failure. #SREcon

> Some useful questions in the operation phase: Do we know if we're currently under attack? Do we know what they're after? Can we turn services off if needed? #SREcon


## <a name="barron"></a> Failure is Not an Option! SRE Lessons 50 Years after the Apollo 13 Flight to the Moon

[Robert Barron](https://twitter.com/flyingbarron) (IBM)

**Twitter threads:**
[cornazano (me)](https://twitter.com/cornazano/status/1336400278833291273)
| [richburroughs (Rich Burroughs)](https://twitter.com/richburroughs/status/1336398888652005379)

**My livetweet contents**

> Going to just sit back and enjoy this talk by @flyingbarron.
>
> #SREcon

> I like the term "self-orchestration", may need to adopt it. #SREcon

> There's an illustration of an oxygen tank temperature gauge here that topped out at 27 C, and didn't reveal going above 500 C. It's a nice illustration of visualization camouflaging the state of the system - relating back to @jpaulreed's talk this morning. #SREcon


## <a name="charagondla"></a> The Good, the Bad and the Ugly: The 3 Learnings of an SRE

[Prathyusha Charagondla](https://twitter.com/pcharagondla) (Adobe)

**Twitter threads:**
[cornazano (me)](https://twitter.com/cornazano/status/1336410822298505224)

**My livetweet contents**

> Next up is @pcharaondla sharing "The Good, the Bad, and the Ugly: The 3 Learnings of an SRE" #SREcon

> First lesson: take a proactive approach rather than a reactive approach.
>
> Reactive approaches result in less productivity. #SREcon

> As part of these proactive approaches we build tools to prevent outages, minimize impact, and reduce toil. Chaos engineering and gamedays also help us to learn about our systems. #SREcon

> Second lesson: pursue effective incident management.
>
> This takes clearly defined roles, including who to involve during an incident, including documentation of what occurred so we can improve and scheduling the postmortem. #SREcon

> I like this: comparing an incident to a play, thinking about the structure of the plot. #SREcon

> Third lesson: need monitoring coverage.
>
> This enables faster detection and understanding of the problem, allowing us to react appropriately (using SLIs/SLOs/SLAs). #SREcon

> There's a spectrum in monitoring. Too little, you have gaps that extend detection time. Too much, and you have too many alarms and produce alerting fatigue. We're looking for the sweet spot between the two, focusing on things that affect our customers. #SREcon

> We need to regularly audit what we're monitoring and alerting to keep this aligned with current needs. #SREcon

> Fourth lesson: we need outside perspectives.
>
> It results in less bias, more innovation, and allows us to change the status quo. #SREcon


## <a name="nauda"></a> Production Population Control: My Cattle are Rabbits!

[Alex Nauda](https://twitter.com/alexnauda) (Nobl9)

**Twitter threads:**
[cornazano (me)](https://twitter.com/cornazano/status/1336417130762395648)
| [richburroughs (Rich Burroughs)](https://twitter.com/richburroughs/status/1336417021190426624)

**My livetweet contents**

> Next up: @alexnauda helping us control the population of our environments. #SREcon

> We've moved from pets, to cattle... to rabbits. With modern cloud-native and Kubernetes approaches, it's really easy to spin things up and then forget about them. #SREcon

> How many prod environments do we need? We end up with many: one per region, maybe multi-cloud, maybe DR, blue/green?
>
> But most of these have sparse traffic at most times. #SREcon

> How many test environments do we need? Team development? Individual developer? CI?
>
> Almost all of them have low traffic as well. #SREcon

> This gets expensive, overstimulating if we monitor/alert on them all the time. #SREcon

> Some good properties of SLOs for these prolific, low traffic environments.
>
> * low context 
> * easily tunable 
> * automatable (SLOs as code)
>
> #SREcon

> What do we use as SLIs? It can't be based on user traffic, there isn't enough.
>
> Instead, we can use occurrence-based slos, lights-on behavior, and synthetic checks. #SREcon

> To get SLOs that self-correct for low traffic, we can use event-based SLIs - measuring ratio of successful events -rather than time based. #SREcon

> Lights on behavior checks look at whether things are on. We can do this with metrics out of kubernetes at the infra level, and can do the same type of check for applications. #SREcon

> Synthetic checks allow us to determine whether the environment is usable even if nobody is actually using it.
>
> Synthetics for applications requires automated functional tests, but can then run and tell us if the environment is behaving correctly. #SREcon

> Recommendation: run these everywhere, even if it's dialed down - we can have a much lower target for environments that are earlier in the pipeline, and strict targets in production. #SREcon

> Individual developer environments should be owned by the developers. For shared environments, consider assigning a rotating role among the people using it. #SREcon

> There are some "production" environments that are business critical, but not at all times. For example, a sales demo environment that isn't used outside of working hours. #SREcon


## <a name="roy"></a> Heap Optimization for Go Systems

Nishant Roy (Pinterest)

**Twitter threads:**
[cornazano (me)](https://twitter.com/cornazano/status/1336423401339105285)

**My livetweet contents**

> Closing out the day listening to Nishat Roy talking about heap optimization in Go.
>
> I'm less familiar with this than with some of the other topics, so I'm going to mostly listen rather than trying to livetweet this one. 
> 😁
>
> #SREcon


# Day 3: Tuesday 2020-12-09

## <a name="guichard-so"></a> Soft Failures, Hard Goals - Accelerating Payments at Scale During the Pandemic

[Kyle Guichard](https://twitter.com/kylesj) (Bill.com)
| Venus So (Bill.com)

**Twitter threads:**
[cornazano (me)](https://twitter.com/cornazano/status/1336687546009608197)
| [richburroughs (Rich Burroughs)](https://twitter.com/richburroughs/status/1336686970429263874)

**My livetweet contents**

> First talk for the day here at #SREcon: @kylesj and Venus So, talking with us about "Soft Failures, Hard Goals - Accelerating Payments at Scale During the Pandemic".

> They work at http://bill.com, and are starting with an overview of the challenges they faced at the beginning of the pandemic. #SREcon

> Initial impacts:
>
> * Increased load on the platform as people moved more of their activity online.
>
> * Switched immediately to remote operations, 24/7.
>
> * Increased reliance on cloud vendors.
>
> #SREcon

> They needed to continue to innovate and deliver new features, but also saw an unacceptable increase in client-facing incidents.
>
> As part of this, they noticed a shift from tribal knowledge to doc & procedures. #SREcon

> Payment processing relies on batch processing, and they were adding new payment options for this. #SREcon

> They practice extreme ownership - this means that teams own everything, including things that are typically outside of their roles (touching automation, for example). #SREcon

> "There are no bad teams, only bad leaders" (quoting Willink & Babin) #SREcon

> As an example of this, sharing a story of a product manager stepping up into a technical lead role - and the importance of making it safe for people to do this! #SREcon

> With the importance of the payments process for them, the decided to treat resilience as a project, meaning it needs: driver, mission, principles, strategy, timelines, and a target.
>
> This helped them instill more dedication to the mission of handling payments.
>
> #SREcon

> They identified 6 tracks with a specific timeline (90 days), and set a target of 40 days without customer impact.
>
> They focused on these tracks as a way to avoid "boiling the ocean" - you can't do everything, so they made sure they picked areas they considered critical.
>
> #SREcon

> Expect to bring people together in cross-functional activities to execute on this type of project. This includes identification of components, needed alerts, and game days. #SREcon

> They needed to build new test automation in their QA teams, and improved unit testing - including a check that required unit tests for check-in. They also worked on design approaches that assume failure. #SREcon

> "You really need to be paranoid to work in this type of process." (paraphrase) #SREcon

> These efforts allowed for *soft failures* - failures that are not a crisis for their team or for their customers. #SREcon

> Their focus allowed them to survive and, better, thrive in 2020. They recently reached 152 incident-free days. (Remember that 40 day target they set) - and this in spite of February being their worst month in terms of incidents. #SREcon

> This is a great question --> "Did we discover the problem before our customers?" #SREcon

> Operational tooling was a problem; they needed to get to a common understanding across teams about what the state of the system is. #SREcon

> As we moved into the pandemic, they needed to improve on collaboration. This requires what feels like overcommunication - hop on a video call if clarity isn't immediate. #SREcon

> They had never executed a business continuity plan, and worked on this. Some things come to the foreground during the pandemic: things like business impact analyses (vendor issues are still your issues) and crisis communication plans. #SREcon

> The economic situation in the pandemic increased the need to think about whether vendors had enough cash to actually survive it. What happens if we depend on a vendor that goes out of business? #SREcon

> Book recommendations, which are influencing their next steps and development of a capability model:
>
> * The Manager's Path (Fournier)
>
> * Extreme Ownership (Willink & Babin)
>
> * An Elegant Puzzle (Larson)
>
> #SREcon


## <a name="shekhar-can-kurt"></a> Hot Swap Your Datastore: A Practical Approach and Lessons Learned

[Raj Shekhar](https://twitter.com/ilunatech) (Quantcast)
| Mehmet Can Kurt (Quantcast)

**Twitter threads:**
[cornazano (me)](https://twitter.com/cornazano/status/1336698833686962180)

**My livetweet contents**

> Next talk is "Hot Swap Your Datastore", by @ilunatech and Mehmet Kurt. #SREcon

> Context: Quantcast offers real time auctions for buying and selling online advertising impressions. #SREcon

> They handle 3.3 million requests/second, and try to handle all requests in under 80 milliseconds. The largest region handles 1.8 million requests/second.
>
> This processing relies on a key-value service containing cookie data, named Keebler; ran one per region. #SREcon

> They decided to replace Keebler. Why? 
>
> * lots of machines and high infra cost;
> * operational complexity (for example, manual resharding);
> * unreliable performance.
>
> #SREcon

> In addition to technical issues (iops limits, long tail latencies, indirect costs in compute clusters), they were experiencing a loss of institutional knowledge about the service.
>
> [Renewal of expertise is a hard problem to solve in most orgs!]
>
> #SREcon

> They chose to use Aerospike (it met their needs well), but the techniques for migrating to this new datastore are not specific to that technology. #SREcon

> Their main requirements for the migration:
>
> * be able to switch back;
> * run in hybrid mode;
> * keep costs down while running in parallel;
> * verify data correctness between two;
> * equal or better latency performance; and
> * no downtime.
>
> #SREcon

> To achieve the reversibility requirement, they used feature flags as a way to enable rollbacks.
>
> Supporting hybrid mode required having full operational support for both, but enabled sequencing the cutover of the regions.
>
> #SREcon

> To verify the correctness of the data, they performed lookups in both Keebler and Aerospike, and logged some of the results in order to verify that the results were consistent. #SREcon

> Since they were in hybrid mode, they were able to kill Aerospike clusters over the weekend. Once they started the actual cutover process, they were also able to reclaim machines from the Keebler clusters. This helped them manage costs. #SREcon

> To verify the latency, they initially had the client receive their results from Keebler while they were verifying the latency of the Aerospike responses. They'd set up dashboards to monitor go/no-go criteria, and they used it extensively here. #SREcon

> The requirement to have no downtime was achieved using a combination of techniques:
>
> * changes were made gradually (by host, using a canary rack, one region at a time);
> * maintained operational support for both for a period of time; and
> * tested rollback processes.
>
> #SREcon

> After this work: Latency is more consistent, and they dropped to about 20% of the previous number of machines. 
>
> Along the way, they also improved their API documentation and integration with Jupyter notebooks.
>
> #SREcon

> Key considerations to accomplish this type of seamless migration:
>
> * Avoid synthetic benchmarks (use production load).
> * Have safety nets (ex: feature flags).
> * Support hybrid mode (smooths the migraiton).
> * Plan rollbacks first.
>
> #SREcon


## <a name="blaho"></a> A Bartender's Guide to Network Monitoring

[John Blaho](https://twitter.com/jpblaho) (Catchpoint)

**Twitter threads:**
[cornazano (me)](https://twitter.com/cornazano/status/1336710164750229513)

**My livetweet contents**

> Next talk: @jpblaho is presenting "A Bartender's Guide to Network Montioring". #SREcon

> He's an amateur mixologist, and as he started onboarding in his new role, he noticed similarities to SRE. There is a focus on getting the right mix to delight your customers, provide them with a repeatable experience, and ensure they keep coming back. #SREcon

> What type of bar would your company be? You need to know your basics because you can't provide the experience if you don't.
>
> [This is a neat question for other customer service industry sectors as well.]
>
> #SREcon

> Know your base. Theme? One-time or repeat customers? How do we create the drink they want?
>
> There are base drinks in mixology, and these are mastered before adapting.
>
> #SREcon

> We need to know the business in order to avoid being reactive. We also need to set expectations appropriately to move to preventative efforts.
>
> Mapping the role to the customer journey can help with this.
>
> #SREcon

> For a bartender:
>
> * The SLA is the cocktail exactly as ordered.
>
> * The SLO is that the recipe and ingredients are available in order to make the drink.
>
> * The SLI is that the customer paid for the cocktail and didn't complain.
>
> #SREcon

> There's a neat discussion here of how real estate has changed in response to the constraints imposed by the pandemic. #SRecon

> Once we know the base, we need to select the right ingredients. What we can do is dependent on what we have available - and this is the source of our challenges and our uniqueness. #SREcon

> For the digital experience, we need to map the dependencies. Designing and modifying this map is the "recipe" that is our path to success. #SREcon

> Don't forget that third-party integrations are part of the experience, and can leave people unsatisfied even if you're portion is good. #SREcon

> Beyond the recipe. The ingredients are there, we have everything, but how do we test it? Is the alcohol still good? Did the soda water go flat?
>
> As an SRE, we need to monitor things over which we don't have direct control, and let ourselves look for better ingredients.
>
> #SREcon

> As we use services in our delivery chain - which are meant to help us - we sometimes end up with reduced visibility and gaps in our ability to understand our increasingly complex systems. The experience cannot be achieved without the bartender (aka SRE). #SREcon

> Shaken not stirred. This is about doing everything right for the experience, based on the previous elements. Think about watching the bartender prepare the drink - we craft a customer experience, not just a drink. #SREcon

> We can go beyond reactive and proactive efforts, and get to a point where we engage with our colleagues to help move away from silos and a better understanding of how teams contribute to the customer experience. #SREcon

> All of this begins by mapping out the different customer journeys. These journeys are the foundation for sharing data and information across the disparate teams that contribute to the organizational effort. #SREcon


## <a name="kuppe"></a> Weeks of Debugging Can Save You Hours of TLA+

[Markus A. Kuppe](https://twitter.com/lemmster) (Microsoft)

**Twitter threads:**
[cornazano (me)](https://twitter.com/cornazano/status/1336721395854831616)

**My livetweet contents**

> Listening to the last talk of the morning now, with @lemmster explaining how "Weeks of Debugging Can Save You Hours of TLA+". #SREcon

> TLA+ is a formal specification language for reactive systems. It allows us to verify the design of a system. #SREcon

> Example incident: a deadlock between producers and consumers, in production for months without change, and never detected in other environments. #SREcon

> To diagnose the problem, we can start with the source code for the producers and consumers, then try to produce with a test. Question: how long do we wait? Is it even *going* to deadlock? #SREcon

> Even if we produce the deadlock, we need a trace of the states the system passes through. Can we even get that without changing the behavior of the system? #SREcon

> While waiting for the deadlock, we can build a TLA+ (Temporal Logic of Actions) specification. The specification includes actions, and we can distinguish between the current state and the next state of the system as part of its properties. #SREcon

> Once we have the spec written, we can start applying tools, like a model checker. Trying it, it doesn't detect the deadlock. We can add a specification requiring no deadlocks as an invariant - and then the checker detects it. #SREcon

> We can even feed different configurations to the model checker to determine under which conditions the system can deadlock. In this case, we find that some configurations are okay, and others can deadlock. This helps us understand behavior during scaling. #SREcon

> We really want something more - we want to understand how we get into the deadlock state. The checker actually produces the shortest trace of states that produce the deadlock! #SREcon

> Understanding the situation via the model lets us identify potential fixes to the deadlock situation. Even better, we can model it in the specification, and test it with the model checker. #SREcon

> We can add more properties - for example, a NoStarvation constraint.
>
> We have two operators we can apply in defining properties: 
>
> [] always 
> <> repeatedly
>
> [These are modal logical operators interpreted in terms of time.]
>
> #SREcon

> Since we're trying to understand correctness, we don't need to care about efficiency in the specification. TLA+ doesn't have the same constraints as the implementation language, but allows us to gain better understanding of what is implemented and validate changes. #SREcon

> Even with small configurations, we find interesting bugs in our code. For stronger guarantees with larger configurations, the TLA+ ecosystem also includes proof systems - but usually we get what we need without investing time in it. #SREcon

> Verification using specification languages supplements implementation languages and tests, they don't replace them. #SREcon

> [Thanks, this was fun! And I blame @hillelogram  for whetting my appetite for this. 😁]
>
> #SREcon


## <a name="chen"></a> Capacity Planning and Performance Enhancement with Page Reference Sampling

Danny Chen (Bloomberg)


## <a name="hahn-hahn"></a> Achieving Mutual TLS: Secure Pod-to-Pod Communication Without the Hassle

Mark Hahn (TBC Technologies)
| Thomas Hahn (TBC Technologies)

**Twitter threads:**

[richburroughs (Rich Burroughs)](https://twitter.com/richburroughs/status/1336739076037177344)


## <a name="jones-hebert-hochstein-huerta-granda"></a> Learning from Adaptations to Coronavirus

[Nora Jones](https://twitter.com/nora_js) (Jeli)
| [Fred Hebert](https://twitter.com/mononcqc) (Postmates)
| [Lorin Hochstein](https://twitter.com/lhochstein) (Netflix)
| [Vanessa Huerta Granda](https://twitter.com/v_hue_g) (Enova)

**Twitter threads:**
[cornazano (me)](https://twitter.com/cornazano/status/1336750574117806090)
| [richburroughs (Rich Burroughs)](https://twitter.com/richburroughs/status/1336749191905722368)

**My livetweet contents**

> Next up is a panel discussion on "Learning from Adaptations to Coronavirus", with @nora_js, @mononcqc, @lhochstein, and Vanessa Huerta Granda. #SREcon

> What are some of the biggest changes you've seen?
>
> Did not have a work from home policy; incident management was based on a physical war room. Using Google meet and docs, Slack for conversation.
>
> #SREcon

> Team was intended to be in a bullpen, relying on ambient conversation. Once it was evident that this was going to be more than a couple weeks, needed to adapt: added more meeting touchpoints, needed to exercise the Slack muscle more, shared docs. #SREcon

> When we entered the pandemic, we entered "safe mode" - make fewer changes for a bit, then adapted to get back to a more typical development cadence. #SREcon

> In contrast: Postmates was already remote-first culture. The hard part here was scaling in the context of suddenly being classified as an essential service, and they were changing cloud providers at the same time. How do we reorganize with new load? #SREcon

> Enova: They have an onsite call center in Chicago. In March, this went remote as well while most call centers in the area were still requiring people to come in. The initial transition was a bit chaotic initially, but it has provided value since. #SREcon

> As a lending company, they had reduced traffic when the pandemic first hit. They were still making changes, though, so they discovered this a bit later as lending picked back up.
>
> Today, teams are more accustomed thinking in terms of resilient systems.
>
> #SREcon

> Postmates: With current COVID case rates, there are no short-term indications that they need to go back to the office. We're working from home *in a time of crisis*, which is different from regular remote work. #SREcon

> Netflix: Were in office, now fully remote. When things move to a hybrid setup (some in-office, some remote), we may find new challenges; some people will have access to communication channels that other people won't. #SREcon

> Postmates: As long as you're 50% remote, most people keep the remote folks in mind. Below that, people stop remembering and there's a quick degradation for the remote workers. #SREcon

> Enova: Initially, working from home is hard. Having a desk with a light makes a difference, and it becomes less bad. #SREcon

> Postmates: Remote work requires us to rearrange how we work. Our new online experiences do not need to be a direct translation of what we do in person - and probably shouldn't be. #SREcon

> Netflix: Getting people to talk about what the bug was is relatively easy; getting them to talk about what they were seeing is harder. #SREcon

> Enova: Re: meeting proliferation. 
>
> Maybe we don't need another meeting, maybe we can just maintain and make sure we check a shared document; for meetings, we're more careful about our agenda.
>
> #SREcon

> Netflix: There are interaction effects (ex: change of a default value in a response) - but it's not certain that we could have caught them with hallway discussions. There is some loss of serendipity, but it's often more about new things rather than changes. #SREcon

> Postmates: Communication is a bit easier to broadcast now. It may be related to scaling-related reorganizations, but the remote tooling facilitates it. #SREcon

> Postmates: Some people are known for writing good incident reports / architecture designs, and this generates more interest in those reports. #SREcon

> [I ended up getting distracted during the second half of this, looking forward to getting to re-watch it once the videos are up.] #SREcon


## <a name="henry"></a> It's a Trap! How Abstractions Have Failed Us.

[André Henry](https://twitter.com/7Grok)

**Twitter threads:**
[cornazano (me)](https://twitter.com/cornazano/status/1336763826763685891)
| [richburroughs (Rich Burroughs)](https://twitter.com/richburroughs/status/1336763799861280768)

**My livetweet contents**

> Closing out the conference, we have André Henry sharing "It's a Trap! How Abstractions Have Failed Us." #SREcon

> What is it? A technique for arranging complexity.
>
> "We can solve any problem by introducing an extra layer of indirection." (David J. Wheeler)
> 
> We need something similar for infrastructure.
>
> #SREcon

> Modern datacenters provide a lot of automation capabilities. For example, hypervisors abstract away hardware system details, allowing multiple operating systems to share it. #SREcon

> Configuration management allows 1-2 people to handle hundreds or thousands of servers, instead of just tens of servers.
>
> With modern virtualization technologies, we start to lose connection with the underlying hardware. #SREcon

> Infrastructure as code wraps everything that came before, and allows us to scale in ways that we couldn't before. We no longer need a large team to scale to large infrastructure. #SREcon

> Why didn't we stop there? There was still something missing: new ways of designing software require new tooling. #SREcon

> We moved into container orchestration, and gained the ability to treat optimization, security, and other parts under one umbrella. #SREcon

> So who benefits? Not all developers grasp all of the abstractions; it's often not part of their core domain.
>
> If they're not using it... Did we do something wrong? Why don't they see the value?
>
> We need to recognize that learning is time consuming!
>
> #SREcon

> Do these abstractions make our jobs easier as SREs? We went from 1:1 relationship between configuration and servers, and it is now 1:many.
>
> We've become managers of ecosystems of complexity.
>
> #SREcon

> Individual developers may not understand what's covered up by the abstractions we use.
>
> [This reminds me of the above-the-line below-the-line model from the Stella report.]
>
> #SREcon

> Claim: we need some balance. We need to do more work before bringing more people into this fragmented ecosystem.
>
> We forgot about our customer.
>
> #SREcon

> We have to explain the limits of our abstractions; the more complex they are, the more difficult this becomes.
>
> We need to document not only the abstraction, but *what the abstraction does*. Does it automatically handle security, or is that up to the application?
>
> #SREcon

> At some point, your team will move on. At that point, your abstraction becomes someone else's problem/code.
>
> How will the abstraction grow with the business needs? It shouldn't be ad-hoc, but needs a plan for how it evolves.
>
> #SREcon

> Despite these abstractions, at some level there is still a real computer. And just because it is out of sight doesn't mean it doesn't exist. 
>
> Every configuration runs on real hardware that embodies tradeoffs.
>
> #SREcon

> We wanted to distribute and democratize knowledge - but we need to acknowledge that we are presiding over silos of knowledge; these silos of expertise - infra, security, etc. - take years to learn and master. #SREcon

> Our abstractions can be difficult to debug. We know that there are limits to everything. If the abstraction doesn't embody this, how do we gain understanding? #SREcon

> Problems stem from the interaction between our code that uses the abstractions, and the underlying systems. If we strip that away, how many of the problems would still exist? What is the cost of extra compute needed just to manage the abstractions? #SREcon

> A lot of our application operational tools start to look like a NOC. Are we getting the benefit we expected? #SREcon

> An important thing to realize is that we are not alone. Automation faces the same types of issues.
>
> What happens when Slack goes away when you depend on chatbots to operate your system?
>
> #SREcon

> Software engineers have also confronted this. We see reactions to this in principles like DRY and YAGNI. But why should we have an interface for something we only call once? #SREcon

> These people are not only our (SRE's) customers, but part of our community. We can reach out and ask them how they draw the lines. #SREcon

> We also need to consider dependency management. Considering the complexity, can we just package them in the JAR? If we can, we can eliminate the problem of not having the right dependency.
>
> Lesson: We should consider the problem we're solving and where it comes from.
>
> #SREcon

> "We need fast provisioning!"
>
> But do we? Some business contexts are predictable, like education systems. In these cases, we can pre-scale based on time rather than demand.
>
> #SREcon

> The question you have to ask yourself: Did you add value?
>
> Are you enabling engineers to be more productive with minimal added overhead and mental load? 
>
> This is a question about the goal you're trying to accomplish.
>
> #SREcon

> Can you use something with less complexity to meet your goals? #SREcon

> Guidance for the future: Consider the root of the problem you're trying to solve? What are the downstream and future impacts? How can we meet SLOs with minimal complexity and overhead? #SREcon
