---
layout: post
title: State of the M&A Market
description: Recent acquisitions represent a huge increase in valuations over historical multiples.
tags: [data, vc]
share: true
---

# tl;dr Recent acquisitions represent a huge increase in valuations over historical multiples.

The recent spat of enormous acquisitions ([Mandiant](http://www.nytimes.com/2014/01/03/technology/fireeye-computer-security-firm-acquires-mandiant.html?_r=0) @ 1B, [AirWatch](http://online.wsj.com/news/articles/SB10001424052702304632204579336310939257846) @ 1.45B, [Nest](http://mashable.com/2014/02/12/google-nest-acquisition/) @ 3.2B, [WhatsApp](http://techcrunch.com/2014/02/19/facebooks-19-billion-whatsapp-acquisition-contextualized/) @ 19B, [Oculus](http://www.wired.com/2014/03/facebook-acquires-oculus/)) in the first three months of 2014 had me question whether this is M&A market is materially different than previous years with the likes of Tumblr @ 1B, Instagram @ 1B, Ariba @ 4.5B, SuccessFactors @ 3.5B and more.  How far outside of normal are we?

I want to start this post with an important caveat.  While [Crunchbase](http://info.crunchbase.com/about/crunchbase-data-exports/) is the most representative public data source for start up information, I've found the fund raising information is more comprehensive than the acquisition data.  For this analysis, I'm assuming (possibly incorrectly) that there aren't any biases introduced by missing data.  Essentially, you need to believe the gaps in either announcement or coverage are uniform across various dimensions (time, category ...).  We'll see at least one example where this assumption might not hold true.

# The Numbers

<figure>
  <a href="{{ site.url }}/images/crunchbase/acquisitions/acquisitions.png"><img src="{{ site.url }}/images/crunchbase/acquisitions/acquisitions.png" /></a>
  <figcaption><a href="{{ site.url }}/images/crunchbase/acquisitions/acquisitions.png" title="Crunchbase Covered Acquisitions">Crunchbase Covered Acquisitions</a>.</figcaption>
</figure>

The number of acquisitions covered by Crunchbase has steadily increased and appears to have reach ubiquity based on a slowing growth rate.

<figure>
  <a href="{{ site.url }}/images/crunchbase/acquisitions/avg_acquisition.png"><img src="{{ site.url }}/images/crunchbase/acquisitions/avg_acquisition.png" /></a>
  <figcaption><a href="{{ site.url }}/images/crunchbase/acquisitions/avg_acquisition.png" title="Avg vs Median Acquisition Prices">Avg vs Median Acquisition Prices</a>.</figcaption>
</figure>

In the beginning of 2014, a few huge transactions are pulling the average up dramatically.  We are clearly outside the realm of normal on the tail of these acquisition prices.  At the same time, the median outcomes haven't moved nearly as much representing that the majority of companies being acquired are more stable.

<figure>
  <a href="{{ site.url }}/images/crunchbase/acquisitions/money_multiple.png"><img src="{{ site.url }}/images/crunchbase/acquisitions/money_multiple.png" /></a>
  <figcaption><a href="{{ site.url }}/images/crunchbase/acquisitions/money_multiple.png" title="Cash on Cash Multiples">Cash on Cash Multiples</a>.</figcaption>
</figure>

Another interesting dimension of these recent acquisitions is the efficiency of investment, the total price of the transaction divided by the total capital raised.  We can see that the current 2014 acquisitions are nearly **4 times** the previous years reported multiples.

## How do you maximize likelihood of an acquisition?

<figure>
  <a href="{{ site.url }}/images/crunchbase/acquisitions/category_acquisition.png"><img src="{{ site.url }}/images/crunchbase/acquisitions/category_acquisition.png" /></a>
  <figcaption><a href="{{ site.url }}/images/crunchbase/acquisitions/category_acquisition.png" title="Category Acquisition Rates">Category Acquisition Rates</a>.</figcaption>
</figure>

Taking a look at rates of acquisition (companies acquired as a percent of all companies not including IPOs), we see that as expected this varies dramatically across categories.  Web, Ads, Gaming and Enterprise lead likely due to lower priced acqui-hires.  Interestingly, Hardware has dramatically lower rates.  While this may be a virtue of the hardware industry dynamics, I suspect this is actually a violation of our assumption that the data coverage is universal.

<figure>
  <a href="{{ site.url }}/images/crunchbase/acquisitions/category_year_acquisition.png"><img src="{{ site.url }}/images/crunchbase/acquisitions/category_year_acquisition.png" /></a>
  <figcaption><a href="{{ site.url }}/images/crunchbase/acquisitions/category_year_acquisition.png" title="Category Acquisition Rates Over Time">Category Acquisition Rates Over Time</a>.</figcaption>
</figure>

Enterprise acquisition rates have been higher than consumer historically.  In 2009, this trend seems to reverse and consumer outperforms.  This could be a reflection of the acqui-hire dynamics or this could be that enterprise acquisitions take longer.

Note that this downward trend is to be expected.  Companies take time to reach an acquisition.  Below we will see it takes between 4 and 5 years to sell.

<figure>
  <a href="{{ site.url }}/images/crunchbase/acquisitions/avg_category_acquisition_lifetime.png"><img src="{{ site.url }}/images/crunchbase/acquisitions/avg_category_acquisition_lifetime.png" /></a>
  <figcaption><a href="{{ site.url }}/images/crunchbase/acquisitions/avg_category_acquisition_lifetime.png" title="Category Lifetime">Category Lifetime</a>.</figcaption>
</figure>

Average time before an acquisition is increasing for both consumer and enterprise companies.  Enterprise companies consistently have a longer time prior to an acquisition.  (Note: this might be a virtue of increased coverage of companies in more recent years.)

# Takeaway

As written about by Redpoint partner Tom Tunguz in this great post about tech [consolidation](http://tomtunguz.com/tech-consolidation/), the large tech companies have huge reserves of cash.  With Microsoft with 106B in current assets and a new CEO, Apple with 80B, Google with 72B, Facebook with 13B and Yahoo at 5B and a valuable stake in Alibaba (as of last reporting).  That is a lot of dry powder seeking revenue growth generation.  All signs point to increased M&A activity.

## Code and Data

Here is a [R script](https://gist.github.com/jdavidson/9905430) for generating graphs and see [Crunchbase](http://info.crunchbase.com/about/crunchbase-data-exports/) for the raw data.
