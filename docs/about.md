---
layout: page
title: About the Blog
permalink: /about-the-blog/
---

The [Iron Triangle of Software Development](https://www.ambysoft.com/essays/brokenTriangle.html) presents a fascinating problem, which for budget-constrained teams can be summarized as _"On time, stable, and complete.  Pick two."_ 

In other words, according this view, there is a high probability the customer (aka source of product funding) will be disappointed.  In every scenario, including when all expectations are met, organizations should be continuously seeking ways to be more efficient at delivering value effectively.  However, as an organization grows beyond a [two-pizza team](https://martinfowler.com/bliki/TwoPizzaTeam.html), it can become difficult to make meaningful improvements at-scale.

From my experience, one pitfall organizations fall into is by focusing on _adoption_ of practices and/or tooling rather than _outcome_.  For example, adopting "Agile" won't prevent over-commitment, achieving 100% test coverage won't ensure production stability, and "continuous delivery" isn't when weekly release windows are still a thing.

A better approach is to focus on outcome-oriented metrics, such as [DORA's software delivery performance metrics](https://dora.dev/guides/dora-metrics/).  However, achieving meaningful improvement in some organizations can be similar to solving a multivariate equation.

Having experience in roles involving the development, evangelization, and adoption of SDLC practices and tooling has provided me with multiple perspectives on the challenges organizations face when attempting to improve.  

This site intends to be more than just a reiteration of best practices - excellent resources already exist, such as the [DORA Capability catalog](https://dora.dev/capabilities/).  Instead, it explores the following questions:

1. Which changes should be made first?
2. Where is energy being wasted?

## Prioritizing Improvements
Unit test coverage minimums, code review gates, and frequent releases are targets organizations may pursue to become more effective at delivering software.   However, the benefits from these may not be as expected if a wider view on the organization is not taken into consideration.  For example:
* What percentage of production incidents have been caused by uncovered code, compared with unsuitable test environments or human error during deployment?
* Will (human) code reviewers rubber-stamp their approvals?
* Are there any obstacles to achieving daily releases, such as mandated change review meetings, or tight coupling with slower-moving components?

There is a cost to making improvements. Ensuring each investment is targeting a verifiable need with a measurable outcome will yield a better result compared with adopting a practice and hoping for a good outcome.


## Conservation of Energy
What does _efficiency_ mean in the context of software development?  The [DORA software delivery performance metrics](https://dora.dev/guides/dora-metrics/) describes what 'good' looks like, however organizations struggling to gain traction on this may want to take a broader and more distilled view of efficiency.

Consider a software delivery ecosystem as being a closed system which includes all of the technical and human participants needed to build and deliver something functional.  Now consider funding as being one form of energy and the value of a delivery as another.  Applying the [law of conservation of energy](https://en.wikipedia.org/wiki/Conservation_of_energy), the efficiency of the ecosystem is how well it converts funding into value.  Less efficient ecosystems will experience a higher degree of loss in the form of delays, instability, and/or incomplete functionality.

This distinction allows for introspection of the entire ecosystem to understand how energy is being applied.  Is it advancing creative and other high-value activities, or being dissipated through procedural meetings, waiting, facilitation, rework, toil, support, context switching, debugging, etc.?   Addressing the foundational issues in the delivery ecosystem will lead to improvements in the DORA metrics.

## The Impedance Mismatch Analogy
The term _impedance mismatch_ represents a loose analogy of the challenges facing development teams, especially in larger organizations.  Its interchangeable with developer friction, as both represent an unexpected resistance when trying to get something accomplished.  That's the gist. 

In electronics, _impedance_ is resistance to an alternating current, such as a radio signal.  When two components carrying the signal (e.g. transmitter and load) have different impedances, this is called an _impedance mismatch_, and a portion of the signal is reflected back to the source. See [Standing Wave Ratio (SWR)](https://en.wikipedia.org/wiki/Standing_wave_ratio).   

Left unchecked, putting too much power through the line will fry the transmitter.

Organizations may have multiple "components" (technical and organizational) involved in the process of delivering software, each with its own impedance (way of working).   When alignment and simplification of the entire process isn't practical, the next-best approach is to [tune](https://en.wikipedia.org/wiki/Antenna_tuner) the circuit to minimize resistance and direct energy towards the delivery of value.




