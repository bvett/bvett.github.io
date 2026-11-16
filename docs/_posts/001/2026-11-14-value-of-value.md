---
layout: post
title:  "The Value of Value"
date:   2026-11-12 17:00:00 -0400
categories: update
---

Chase value, not metrics.
<!--more-->

### Goodhart's Law

To see [Goodhart's Law](https://en.wikipedia.org/wiki/Goodhart%27s_law) in action, observe a large organization attempting to improve the quality and velocity of its software delivery.  This might involve a centrally-managed "transformation" program driving teams towards the adoption of different practices and/or achieving a target measure. For example:
* _xx% code coverage_ 
* _99.999% service uptime_ 
* _Daily releases_ 
* _"Agile"_
* etc...

The problem arises, as Goodhart's Law summarizes, when achieving the measure becomes confused with the desired outcome.  Examples of how the measures above could miss the intent:
* Code coverage: high-coverage/low-quality tests fail to catch errant code changes.
* Service uptime: measurement can vary, especially for distributed multi-tenant services.
* Daily releases: exposes bottlenecks further along the development pipeline (like manual user-acceptance and change review processes) that are beyond the program's scope. 
* Agile adoption: maintaining a waterfall process with an Agile façade.  

To be clear, improved practices should yield improved outcomes, and measurement is essential for improvement.  So what should be measured?  

### Value and Loss

At a high-level, every feature has an expected value to a customer or the organization itself.  The function of software development is to "deliver value" by actualizing features.  It's a project planning cliché to say the customer "wants it yesterday," but this just expresses how the value begins to depreciate from the moment an opportunity is identified.  A feature intended to capitalize on a business opportunity may wind up being worthless if delivered late.

_Loss_ is the depreciation of value (expressed as a percentage) from when a feature is identified to when it is put to use.   An effective software delivery ecosystem therefore is one which minimizes loss and maximizes the _value stream_. This enables an assessment of the _outcome_ independent of the processes, methods, and technologies used to achieve it.

Why not use _time to market_ (TTM)?

TTM and loss are related, and similar results could be achieved by using [_lead time for changes_](https://dora.dev/guides/dora-metrics/) instead.  Loss has the advantage of being a broader measure; whereas lead time for changes measures the time from code commit (aka dev-complete) to running in production, loss also reflects:
* pre-commit factors, such as prioritization schemes and developer environment friction.
* post-production factors, such as stability and outages.

### Example

Value can be visualized using the [Value Stream Simulator](https://github.com/bvett/value-stream-simulator):

This simple example demonstrates a single developer working on 30 tasks (features), each with the same initial value and no depreciation:

![No Depreciation](/images/001/000-depreciation.png)

Without depreciation, there is no loss regardless of how (in)frequently features are delivered.

With an arbitrary 1% depreciation applied, it becomes clear that loss is reduced with increased deployment frequency:

![Depreciation](/images/001/010-depreciation.png)

Now it becomes possible to evaluate the impact of changes.   Let's see how loss is affected when our solitary developer needs to spend 10% or 50% of their time on support work:

![Support](/images/001/010-depreciation-with-support.png)

While this example is rather simplistic and contrived, it shows how using loss can inform decision-making.  In this case, reducing the deployment interval from t=7 to t=0 would result in an approximate 3% reduction in loss, but for this hypothetical project efforts would be better spent getting support under control as it would yield a greater (~10%) improvement to the value stream.




