---
layout: post
title: Enterprise vs Consumer Start Ups
description: Enterprise is the bread and butter of venture with good reason
tags: [data, vc, crunchbase]
share: true
---

# tl;dr Enterprise is the bread and butter of venture with good reason

Looking at tech press on publications like TechCrunch, PandoDaily, and GigaOM, you might expect that consumer start ups are the only thing that matters in the early stage technology industry.  I expect this trend is due to consumer start ups being easier to grok for an increasingly diverse readership.  Articles about companies with products selling to or targeting consumers, serve as both advertising as well as news.

In Aileen Lee's great Unicorn Club [post](http://techcrunch.com/2013/11/02/welcome-to-the-unicorn-club/), she cites the broad success of consumer companies both in terms of numbers as well as out-sized successes (which has only grown with success of Twitter and Zulily IPOs).  This is a great analysis of the handful of companies that make it to this stage but isn't necessarily representative of the broader start up landscape and suffers from a survivorship bias.

Taking a broader look at aggregate fund raising data, enterprise still has the lion share of interest and activity.  [Tom Tunguz](http://tomtunguz.com/consumer-web-investing/) takes a look at the NVCA data.  >> "This massive swing toward enterprise investing never existed. It’s a fallacious perception. Enterprise investing has always been the norm and will continue to be for quite some time."

As I dive further into venture, I wanted to get a sense for the different dynamics for these categories.  As I have used [before]({{ site.url }}/how-much-to-raise-using-crunchbase-data/), one empirical measure of start up success is the likelihood of a follow on round.  It is flawed but hopefully directionally accurate metric for start up success.

# Category comparison

<figure>
  <a href="{{ site.url }}/images/crunchbase/category-follow-on.png"><img src="{{ site.url }}/images/crunchbase/category-follow-on.png" /></a>
  <figcaption><a href="{{ site.url }}/images/crunchbase/category-follow-on.png" title="Category follow on rates over time"></a>Category follow on rates over time.</figcaption>
</figure>

## Takeaway

The average enterprise start up is more likely to raise a subsequent round.  This naturally does not account for the size of a success.  Combined with Aileen's analysis this is in support of the perception that consumer start ups are closer to a lottery ticket.  There may be a smaller chance of success but the potential for enormous scale.

## Code and Data

Here is a [R script](https://gist.github.com/jdavidson/8789695) for generating graphs and see [Crunchbase](http://info.crunchbase.com/about/crunchbase-data-exports/) for the raw data.
