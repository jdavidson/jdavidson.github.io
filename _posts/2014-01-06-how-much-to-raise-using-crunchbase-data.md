---
layout: post
title: How much to raise using Crunchbase data
description: Raise enough to hit the next milestones to raise the next round plus a healthy buffer.
tags: [data, vc]
image:
  feature: coins.jpg
share: true
---

tl;dr Raise enough to hit the next milestones to raise the next round plus a healthy buffer.

After starting PrimaTable in 2011, raising a seed round and selling to Hotel Tonight and now sitting on the other side of the table, I've been asked: How much venture funding to raise?  Fund raising can be more art than science with a competitive process that dictates terms.  In this post, let's take a quick look at the data.

It's been written about before:

1. [Tom Tunguz](http://tomtunguz.com/most-important-principle-of-fund-raising/)
    "Raise enough money to achieve a set of milestones that will attract a subsequent round of investment from new investors.”

2. [Mark Andreessen](http://venturehacks.com/articles/how-much-money)[^1]
    “Raise as much as you can without giving away control of your company, and without being insane. ... In a normal scenario, raising more money rather than less usually makes sense, since you are buying yourself insurance against both internal and external potential bad events."

Thanks to [Crunchbase](http://info.crunchbase.com/about/crunchbase-data-exports/), there is data to examine.

## The Numbers

<figure>
  <a href="{{ site.url }}/images/crunchbase/cumulative_distribution_first_raised_amount_usd.png"><img src="{{ site.url }}/images/crunchbase/cumulative_distribution_first_raised_amount_usd.png" /></a>
  <figcaption><a href="{{ site.url }}/images/crunchbase/cumulative_distribution_first_raised_amount_usd.png" title="Cumulative Distribution of First Round Amount">Cumulative Distribution of First Round Amount</a>.</figcaption>
</figure>

Looking at the distribution of the first round amount (restricting to only recent companies first funded between 2010 and 2013), the median is $1.2M with few extreme outliers.  While this itself is informative, further funding history is a layer deeper.  Raising a subsequent round can be viewed as a signal for some success, as other people have done ([Benn @Mode](http://blog.modeanalytics.com/are-stanford-grads-good-investments/)).[^2]

<figure>
  <a href="{{ site.url }}/images/crunchbase/follow_on_by_first_raised_amount_usd.png"><img src="{{ site.url }}/images/crunchbase/follow_on_by_first_raised_amount_usd.png" /></a>
  <figcaption><a href="{{ site.url }}/images/crunchbase/follow_on_by_first_raised_amount_usd.png" title="Follow On by First Funding Amount">Follow On by First Funding Amount</a>.</figcaption>
</figure>

There seems to a positive correlation between the initial fund raise amount and the likelihood of a follow on round. Note, this is clearly an instance of correlation and not necessarily causal. The companies that raise more money may be more likely to succeed or better able to raise a subsequent round of funding. There are likely exogenous factors that influence follow on rounds. However, the relationship makes sense. In order for it to also reflect the collective wisdom on fund raising, the relationship should demonstrate a very specific activity based on individual company dynamics.

<figure>
  <a href="{{ site.url }}/images/crunchbase/follow_on_by_first_raised_amount_usd_by_category.png"><img src="{{ site.url }}/images/crunchbase/follow_on_by_first_raised_amount_usd_by_category.png" /></a>
  <figcaption><a href="{{ site.url }}/images/crunchbase/follow_on_by_first_raised_amount_usd_by_category.png" title="Follow On by Category">Follow On by Category</a>.</figcaption>
</figure>

Decomposing fund raising impact further by category, the positive correlation in general persists but varies dramatically by category. In many categories, Biotech, Cleantech, and Software, there is no explicit relationship.  Companies that have raised larger initial rounds haven't converted to a second round at a greater rate.  In the case of Mobile, the relationship is the inverse.  Mobile companies that have raised more are in general less likely to raise a follow on round.

### Median First Raised Amount
<figure>
  <a href="{{ site.url }}/images/crunchbase/medians.png"><img src="{{ site.url }}/images/crunchbase/medians.png" /></a>
</figure>

In addition to differing relationships with additional funds, the aggregate amounts across category varies.  The median amount raised when conditioning on follow on rounds varies wildly.  In ecommerce, the median first round for companies that raised a further round is $1.3M vs just $.5M for companies that haven't.

## Takeaways

This data can help substantiate the thesis that you should raise enough to hit the next milestones and mitigate risk with a sufficient buffer to weather the inevitable bumps. Valuation for startups only increases on mitigation of risk. For example, in some seed stage companies, this can mean mitigating technical risk and building a working product. For a series A, this might mean finding product market fit and showing user engagement. For later stages, this can be demonstrating a scalable distribution channel and business model. Regardless of the stage, future rounds will necessitate mitigation of risk.

Mark argues to mitigate financing market risk by raising at the max of the range that is possible. This make sense to protect against macro changes that change fund raising dynamics as well as gives as much fuel to hold on as long as possible. This can be detrimental because this ups the level of risk that must be mitigated prior to a subsequent round.

In practice, for most early stage startups, the increments of funding look to be 12 - 18 months of runway. The round size varies with the team but you can use a [rule of thumb](https://angel.co/salaries) of $125K / developer / year ($100K salary + 25% expenses).

In summary, raise enough to hit the next milestones plus a healthy buffer.

## Code and Data

Here is a [R script](https://gist.github.com/jdavidson/8287656) for generating graphs and see [Crunchbase](http://info.crunchbase.com/about/crunchbase-data-exports/) for the raw data.

[^1]: As quoted on Venture Hacks from an old post subject to [link rot](http://en.wikipedia.org/wiki/Link_rot).
[^2]: This neglects bootstrapped companies, companies that reach profitability or companies that sell, not requiring subsequent financing.
