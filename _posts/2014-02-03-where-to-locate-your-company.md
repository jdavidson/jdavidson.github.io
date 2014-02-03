---
layout: post
title: The best place to locate your start up
description: Empirically, SF is better for early success than Silicon Valley for a start up
tags: [data, vc, crunchbase]
share: true
---

# tl;dr Empirically, SF is better for early start up success than Silicon Valley

In my last [post]({{ site.url }}/where-start-ups-are-raising-vc/), I presented a visualization of the geographic distribution of start up fund raising.  While observing fund raising is becoming more geographically diverse, SF grew dramatically.  There are a number of reasons why this is the case.  First, let us dive into an empirical look at the likelihood of a follow on round, a flawed but hopefully directionally accurate metric for start up success (discussed [here]({{ site.url }}/how-much-to-raise-using-crunchbase-data/)).

## Where should start ups locate?

Below is a chart taking a look at the four largest US start up regions, SF Bay Area, New York, Boston and Los Angeles.  Surprisingly, Boston consistently has the most "successful" start ups, as measured by follow on rate.  While it's larger than the Bay Area and NY, they are not materially different (mostly within 5-10%).  Los Angeles is consistently the lowest.

<figure>
  <a href="{{ site.url }}/images/crunchbase/region-follow-on.png"><img src="{{ site.url }}/images/crunchbase/region-follow-on.png" /></a>
  <figcaption><a href="{{ site.url }}/images/crunchbase/region-follow-on.png" title="Geographic region follow on rates over time"></a>Geographic region follow on rates over time.</figcaption>
</figure>

The prevailing wisdom of the venture community has been "I'm not sure you can build a great technology firm outside of the Bay Area".  Examples like Tumblr, Groupon, Gilt, Etsy, Amazon ... (the list goes on) demonstrate it isn't impossible.  Starting outside of Silicon Valley is just harder.

A lot has been written about why silicon valley is so special.  Start ups are a network effect business.  The community is a tremendous helpful one where coffee meetings and friendly referrals are common.  As a founder the network of potential employees, investors, and customers is essential.

[Paul Graham](http://paulgraham.com/hubs.html)
>> "being in a place where startups are the cool thing to do, and chance meetings with people who can help you. And what drives them both is the number of startup people around you."

[Maxwell Wessel](http://blogs.hbr.org/2013/10/dont-build-your-startup-outside-of-silicon-valley/) at HBR
>> "But the reality for entrepreneurs outside of the established startup meccas is a difficult one: if you start a technology business somewhere other than the San Francisco Bay area, New York, or Boston, you’re stacking the deck against yourself."

Beyond the immediate benefits of the tech community, the cultural focus on technology as an enabler and disrupter turns San Francisco into a place much like Paris in the 1870s and 1880s.  With a critical mass of radical artists in Paris, Impressionism grew because of a culture of freely flowing ideas.  Similarly, for better or for worse, you can't walk into a coffee shop in SF without over hearing a start up pitch, brainstorm or critique.

## SF or the Valley?

In the last few months, I've spoke with a number of portfolio companies and start ups just getting off the ground that are struggling with where to locate within Silicon Valley.  The common wisdom is it is easier to recruit young engineering talent in SF (where they live) but as a company grows and the work force ages it might be best to locate down south (where the school system is better).  It has been [argued](http://m.theatlanticcities.com/jobs-and-economy/2013/08/why-san-francisco-may-be-new-silicon-valley/6295/) that San Francisco is the new Silicon Valley.  Indeed, we've [seen](({{ site.url }}/where-start-ups-are-raising-vc/)) a dramatic increase in capital raised in SF in the last few years.

The figure below shows that SF has been consistently better than the broader silicon valley.  This success may be partially why the center of gravity has shifted.  I based my company, PrimaTable, in SF (although admittedly for convenience and not due to any analysis).

<figure>
  <a href="{{ site.url }}/images/crunchbase/sf-follow-on.png"><img src="{{ site.url }}/images/crunchbase/sf-follow-on.png" /></a>
  <figcaption><a href="{{ site.url }}/images/crunchbase/sf-follow-on.png" title="SF Bay Area follow on rates over time"></a>SF Bay Area follow on rates over time.</figcaption>
</figure>

## Takeaway

Now we know why [all roads lead to San Francisco]({{ site.url }}/where-start-ups-are-raising-vc/).  San Francisco has a consistently better success rate for start ups.

Time for my standard disclaimer, this analysis reflects correlation and not causation.  There could be a wide variety of reasons that start ups that are more likely to succeed are predisposed to start in specific geos.  For any group of start ups so motivated, I'd be happy to help construct a semi-natural experiment to observe the true causal effects of geography.  Call it the A/B test for start ups.  Although, I have to caution, I wouldn't recommend it :).


## Code and Data

Here is a [R script](https://gist.github.com/jdavidson/8786950) for generating graphs and see [Crunchbase](http://info.crunchbase.com/about/crunchbase-data-exports/) for the raw data.