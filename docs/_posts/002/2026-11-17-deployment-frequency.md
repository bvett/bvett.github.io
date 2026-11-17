---
layout: post
title:  "Why Deployment Frequency Matters"
date:   2026-11-17 12:00:00 -0400
categories: update
---

Why wait? Ship!

<!--more-->

A lot has been written over the past 10+ years about continuous delivery, with deployment frequency being one of [DORA's software delivery metrics](https://dora.dev/guides/dora-metrics/).

A [previous post](/articles/value-of-value) introduced the idea of using value and loss as a way to measure the effectiveness of software delivery.  In this article, we'll apply this to deployment frequency.

Using the [Value Stream Simulator](https://github.com/bvett/value-stream-simulator), we can put together a simulation that compares the net loss across team sizes (1, 3, 5, and 10) and deployment intervals (t=0, 1, 7, 14, and 30):

![Baseline](/images/002/baseline-no-annotations.png)

Unsurprisingly, this shows that loss is reduced by increasing the release frequency, as does having a larger development team ... to a point.

Lets look at how much loss is reduced across deployment intervals when 9 developers are added to the team:

![Convergence](/images/002/convergence.png)

This shows how the benefit of extra developers is maximized with higher deployment frequencies.  In this simplistic scenario, while larger teams complete the tasks sooner, the tasks continue to lose value while waiting for the next deployment to occur.

An organization might be inclined to add more developers in order to increase velocity, but as this view demonstrates, it's important to look broadly at the entire development ecosystem for other opportunities.

Let's zoom in a little bit for an example:

![Zoomed](/images/002/zoomed-annotated.png)

Here, a team of 3 developers (top line) releasing every t=7 results in a loss of 9.33%.   Adding 2 or more developers to the team (bottom line) reduces loss by 2.54%.  However, by changing practices to release every t=1, loss is reduced by 3.05% - a greater improvement at a potentially lower cost.

For organizations looking to benefit from continuous delivery, adopting an automated toolchain is only part of the solution.  Sometimes changing practices is more difficult, and it doesn't have to be due to a lack of willingness. There can be many headwinds to achieving a higher deployment frequency.  These will be explored in future articles.



