---
date: 2019-06-02
title: "Value Stream Mapping References (DevOpsDays Toronto 2019)"
summary: >
  2019-06-02.
  One of the open spaces topics on Wednesday was Value Stream Mapping. During the discussion, several books were mentioned; since people asked for references to them, here we go!
---

One of the open spaces topics on Wednesday was Value Stream Mapping. During the discussion, several books were mentioned; since people asked for references to them, here we go!

---

Karen Martin and Mike Osterling (2014). _Value Stream Mapping: How to Visualize Work and Align Leadership for Organizational Transformation_.

This book describes the process of value stream mapping and how to use value stream maps to improve how we manage value streams. A _value stream_ is "the sequence of activities an organization required to design, produce, and deliver a good or service to a customer" (p. 2), and a _value stream map_ is a visualization of this sequence.

During the session, we talked about the difference between a _current state_ map, which captures how value is currently produced, and a _future state_ map, which shows a vision of how we want to do the same work at some point in the future. Current state mapping is covered in Chapter 3, and the design of a future state in Chapter 4. The remainder of the book discusses some aspects of how to move from the current state to the desired future state.

---

Mike Rother (2010). _Toyota Kata: Managing People for Improvement, Adaptiveness and Superior Results_.

One of the things to keep in mind when moving from the current state to the future state is that we will learn more as we try to move forward. The future state is often designed at the beginning of the change, when we have the least knowledge about how the rest of the system will react to the changes we make. The _improvement kata_ introduced in Part III provides a useful model for learning our way towards the future state, and the _coaching kata_ in Part IV gives some guidance on helping people develop their ability to learn their way through the unknowns.

---

Mik Kersten (2018). _Project to Product: How to Survive and Thrive in the Age of Digital Disruption with the Flow Framework_.

A concern raised during the session was how to get management to allow for necessary improvement work instead of just pushing teams to cut corners. This book introduces the flow framework, which provides a useful model for understanding how to balance among four key types of work: _features_, _defects_, _risks_, and _debt_. It also discusses the business problems that arise when we do not maintain an appropriate balance among these.

(Mik Kersten also discussed these relationships in [his talk at DevOps Enterprise Summit in 2018](https://www.youtube.com/watch?v=E5VP3ioSRU8).)

---

Eliyahu M. Goldratt (1984/2014). _The Goal: A Process of Ongoing Improvement_.

This came up when we were talking about how to decide what to improve in a process. The book is structured as a business fable, and introduces the _theory of constraints_. The key insight here is that the only useful place to improve a process is at the current constraint (the bottleneck). Improving an activity that comes before it will just pile up more work and pressure at the point of the constraint, while improving an activity that comes after it will just leave the activity even more starved for inputs. This can help us determine _where_ to invest time in process improvement, rather than trying to improve everything at the same time.

---

Betsy Beyer, Niall Richard Murphy, David K. Rensin, Kent Kawahara, & Stephen Thorne, editors (2018). _The Site Reliability Workbook: Practical Ways to Implement SRE_.

One of the participants raised the question of how to find time to make improvements. As part of the ensuing discussion, the concept of _toil reduction_ was brought up. Toil, and how to deal with it, is covered in Chapter 6 (also available [online](https://landing.google.com/sre/workbook/chapters/eliminating-toil/)). The core idea here is to start with automation to facilitate the most toil-intensive parts of our jobs. In the flow framework mentioned above, these investments would likely be considered debt. As we make progress on this, it frees up time and capacity to work on other things.

---

Donald G. Reinertsen (2009). _The Principles of Product Development Flow: Second Generation Lean Product Development_.

When we talked about how to prioritize work, the concept of _cost of delay_ came up as something to consider. This book covers several consequences of our use of queues to manage work, and makes use of cost of delay throughout the discussion as a way to help us decide what to work on, and in what order.

---

Melissa Perri (2019). _Escaping the Build Trap: How Effective Product Management Creates Real Value_.

Whenever we talk about value stream management, a frequent question is what we even mean by "value", and it came up multiple times during the session. This book examines value - and how it is created - from a product management perspective. It brings together several of the topics we talked about, including the need to explore both the problem (a current state) and a potential solution (a future state); the need to learn our way forward through unknowns (using a _product kata_); and prioritization of work using cost of delay.
