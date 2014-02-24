---
layout: post
title: Should you raise a seed from institutional VC?
description: Top Institutional VC seed rounds have higher follow on rates than even dedicated seed funds.
tags: [data, vc]
image:
  feature: seed.jpg
  credit: oatsy40
  creditlink: http://www.flickr.com/photos/oatsy40/8923459422/
share: true
---

tl;dr Top Institutional VC seed rounds have higher follow on rates than even dedicated seed funds.

While meeting with early stage companies just getting started, one question I'm often asked: "Should I raise a seed from angels or institutions".

Startups looking at large institutional venture investment in a seed round need to consider signaling risk.  The theory is that as Chris Dixon [says](http://cdixon.org/2009/10/30/the-most-important-question-to-ask-before-taking-seed-money/) "if you were in the seed program of a VC who has a multi-hundred million dollar fund and who decided to pass, that is a huge signal."  If VCs that should know your company the best don't like it enough to follow on, that is a negative signal to other potential investors.

In my experience, companies at a Series A are either doing well and able to raise from multiple investors or aren't and shouldn't.  The risk is real for companies at the margin.  The reason a seed VC doesn't want to follow on can be as simple as a personality mismatch.  As an entrepreneur, you can attempt to mitigate the signaling risk by including multiple funds.

At my startup, PrimaTable, we raised from [three](http://www.gv.com/) [great](http://www.battery.com/) [VCs](http://www.interwest.com/), an excellent seed fund [DCVC](http://dcvc.com/) and a few individuals.  We met with a number of angels and had interest.  Ultimately, we decided to raise funding from VC because it was much more expedient.  Individual funds made a multi hundred thousand dollar decision after two or three meetings.  After a number of meetings with individuals, it was clear that wrangling interest would have been very time consuming.  (Note [Angellist](https://angel.co/) was just starting and could have greatly improved the process).  Fund raising is never the goal, merely a means to build a great company.  We wanted to get back to work and raising institution venture was more efficient.

Let's take a quick look at follow on investment data from [Crunchbase](http://info.crunchbase.com/about/crunchbase-data-exports/).

## Data

Crunchbase provides great funding round data but doesn't have explicit classification for funds.  The data does break up investors into angel, corporate, and financial.  First, individual angels have a consistently higher follow on rate than financial investors.

<figure>
  <a href="{{ site.url }}/images/crunchbase/angel-follow-on-type.png"><img src="{{ site.url }}/images/crunchbase/angel-follow-on-type.png" /></a>
  <figcaption><a href="{{ site.url }}/images/crunchbase/angel-follow-on-type.png" title="Angel Follow On Rate by Investor Type">Angel Follow On Rate by Investor Type</a>.</figcaption>
</figure>

Then let's break financial investors into the 100 most active seed funds, defined by greater than 20% of their investments being an angel round and the 100 most active venture investors.

<figure>
  <a href="{{ site.url }}/images/crunchbase/angel-follow-on.png"><img src="{{ site.url }}/images/crunchbase/angel-follow-on.png" /></a>
  <figcaption><a href="{{ site.url }}/images/crunchbase/angel-follow-on.png" title="Angel Follow On Rate by Investor Class">Angel Follow On Rate by Investor Class</a>.</figcaption>
</figure>

The top funds consistently outperform both the seed funds and angel investors by a healthy margin greater than 10%.  This is surprising to me but can partially be explained by larger funds with the capacity to continue to fund an early stage company.  In practice, the aggregate effect of venture participation in seed rounds is positive.

The rest of the financial funds (after breaking out the top seed and top funds) have dramatically worse follow on rates.  It is perhaps obvious that the top funds would have better performance but again the magnitude is surprising.

## Takeaway

Here we demonstrate that investor classification is correlated to seed performance.  This is not necessarily causal.  Angel investors and seed funds have different risk and reward profiles which will naturally drive different sort of investments.  These could be moon shots that when they hit can be much larger.

My advice to startups raising a seed round is to raise the [right amount]({{ site.url }}/how-much-to-raise-using-crunchbase-data/) at the [right time]({{ site.url }}/when-to-raise-using-crunchbase-data-part-2/) from the right partners in the most expedient way.  Sometimes that will mean institutional VC, sometimes seed funds and sometimes angels.  This will depend on the risk profile of your venture.

## Code and Data

Here is a [R script](https://gist.github.com/jdavidson/9191278) for generating graphs and see [Crunchbase](http://info.crunchbase.com/about/crunchbase-data-exports/) for the raw data.
