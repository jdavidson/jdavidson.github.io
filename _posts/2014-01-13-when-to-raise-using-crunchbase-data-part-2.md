---
layout: post
title: When to raise using Crunchbase data
description: Target raising 9 months after your last raise.
tags: [data, vc]
image:
  feature: clock.jpg
share: true
---

tl;dr the likelihood of a follow on financing peaks at around 9 months.

At Google and later at Hotel Tonight, data that represents actual user activity (search, click, purchase events) is always more valuable than the best academic model. For the venture industry, fundings are the most public activity for start up behavior. Looking at start up behavior and success can inform strategy and [Crunchbase](http://info.crunchbase.com/about/crunchbase-data-exports/) represents a treasure trove of great start up activity data.

In my first post, I took a look at [how much start ups raise]({{ site.url }}/how-much-to-raise-using-crunchbase-data/). I concluded that start ups should target 12 - 18 months of runway. As a follow up, I want to take a deeper look at timing.  The empirical cadence and timing of funding can hopefully inform time lines.

By reconstructing the start ups funding history represented by the crunchbase data, we can observe how likely they are to raise a subsequent round after an initial financing.  Note not raising another round isn't necessarily a negative signal.  For the purpose of this analysis, we'll take a simplifying assumption that start ups below a Series C will require subsequent financing to be successful (reach profitability or acquisition).  Also, Crunchbase represents publicly announced funding.  For this analysis, it is assumed that delays in announcements affect each round equally in aggregate.

## The Numbers

### Median First Raised Amount
<figure>
  <a href="{{ site.url }}/images/crunchbase/medians-time.png"><img src="{{ site.url }}/images/crunchbase/medians-time.png" /></a>
</figure>

Looking at the fraction of start ups that subsequently raise at any point after a number of months after financing, will demonstrate an empirical likelihood.  Start ups at different funding round stages (Angel, A, B ...), should be considered differently as they have different risks and capital requirements.  The median time between rounds increases in subsequent rounds but not by much.  The median successful start up in any round raises after a year.

<figure>
  <a href="{{ site.url }}/images/crunchbase/follow-on-likelihood-by-time.png"><img src="{{ site.url }}/images/crunchbase/follow-on-likelihood-by-time.png" /></a>
  <figcaption><a href="{{ site.url }}/images/crunchbase/follow-on-likelihood-by-time.png" title="Likelihood of Raising a Follow On Round by Time">Likelihood of Raising a Follow On Round by Time</a>.</figcaption>
</figure>

Angel and Venture stage companies behave very similarly and are much less likely than a Series A or B to have a follow on round.  For Angel start ups, the likelihood of raising a subsequent round monotonically decreases with each month from their seed round.  Series A and Bs behave similarly (with As consistently less likely to raise another round at each).  Their likelihood for a subsequent financing peaks at 9 months after financing.  Intuitively, this makes sense.  If start up valuations (and likelihood of fund raising) only increases on mitigation of risk, 9 months seems like the point at which start ups prove their model.  Whether this is a scalable business model, a distribution channel, or product engagement, start ups need to be razor focused on it.  The peak probability of raising is very quickly after your last raise.

The discrepancy between Angel rounds and Series A and B could be explained by differences in the round size.  Decomposing the trends by both round and amount helps eliminate the interaction.

<figure>
  <a href="{{ site.url }}/images/crunchbase/follow-on-likelihood-by-round-size.png"><img src="{{ site.url }}/images/crunchbase/follow-on-likelihood-by-round-size.png" /></a>
  <figcaption><a href="{{ site.url }}/images/crunchbase/follow-on-likelihood-by-size.png" title="Likelihood of Raising a Follow On Round by Amount">Likelihood of Raising a Follow On Round by Amount</a>.</figcaption>
</figure>

Looking first at Angel rounds, the likelihood increases with an increase in the initial funding amount.  While this makes sense, this is correlated and not necessarily causal.  This may be a reflection of the type of companies that command a large seed round.  After the venture and angel rounds, the peak likelihood for Series A is actually $5-10M rounds and the max for Series B is $20-40M.  Interestingly, there is not a clear correlation between round size and likelihood.  It seems like there is a sweet spot in an amount to raise but more isn't necessarily better on later rounds.

<figure>
  <a href="{{ site.url }}/images/crunchbase/follow-on-likelihood-by-round-category.png"><img src="{{ site.url }}/images/crunchbase/follow-on-likelihood-by-round-category.png" /></a>
  <figcaption><a href="{{ site.url }}/images/crunchbase/follow-on-likelihood-by-round-category.png" title="Likelihood of Raising a Follow On Round by Category">Likelihood of Raising a Follow On Round by Category</a>.</figcaption>
</figure>

Finally, let's look across start up categories.  Most categories show similar trends, with the primary difference being the aggregate likelihood (e.g. at month 0 Advertising at ~40% vs Ecommerce at ~30%).  In categories that are about scalable business models, ads, biotech, and enterprise, there is less of a lottery ticket consumer adoption model.  Within these categories, non-seed rounds have a significantly higher likelihood of raising.  Presumably these companies have already proven a business model and value proposition.  They are raising additional funding to scale with the goal of increasing marketing or hiring addition sales people.

For categories, where consumer adoption is the primary risk, mobile, video games and to some extent ecommerce, there seems to be similar risk levels at each round.  These companies either hit it and find a scalable distribution model or don't.  Every month without that hockey stick just eats into the war chest.

In summary, the likelihood of a follow on financing peaks at around 9 months.  As we saw previously, there is a right amount to raise to maximize likelihood of subsequent rounds.  Interestingly, as with funding amount, timing also varies dramatically by category.

## Code and Data

Here is a [R script](https://gist.github.com/jdavidson/8406379) for generating graphs and see [Crunchbase](http://info.crunchbase.com/about/crunchbase-data-exports/) for the raw data.
