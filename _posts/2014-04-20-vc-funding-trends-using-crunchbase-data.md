---
layout: post
title: Recent VC spending peak reflects new pre-IPO rounds
description: Venture financing hit a recent quarterly peak Q1 2014.  This peak is due to a handful of late stage deals in a new pre-IPO environment.
tags: [data, vc]
share: true
---

# tl;dr Venture financing hit a recent quarterly peak Q1 2014.  This peak is due to a handful of late stage deals in a new pre-IPO environment.

With the release of the [NVCA](http://www.nvca.org/) / PriceWaterhouse Cooper [MoneyTree report](https://www.pwcmoneytree.com/MTPublic/ns/index.jsp) last week, a lot has been written about the state of venture financing.

* [Software is eating the world](http://venturebeat.com/2014/04/18/software-is-eating-the-world-and-venture-capital-is-feasting-on-older-software/) says [Kia Kokalitcheva](https://twitter.com/imkialikethecar) at VentureBeat
* [Raise Now](http://techcrunch.com/2014/04/18/raise-now-vc-funding-for-startups-at-highest-point-in-more-than-a-decade/) advises [Alex Wilhelm](https://twitter.com/alex) at TechCrunch
* [Venture Capital Funding Is Nowhere Near Dot-Com Levels](http://www.businessinsider.com/historical-venture-capital-funding-2014-4) cautions [Sam Ro](https://twitter.com/bySamRo) at Business Insider

The focus of the response has been on the top line [reported](https://www.pwcmoneytree.com/MTPublic/ns/moneytree/filesource/displays/notice-D.html).  "Venture capitalists invested $9.5 billion in 951 deals in the first quarter of 2014."  The comparisons drawn have been to past bubbles.

A level deeper, the MoneyTree press release goes on to recognize that this growth didn't come necessarily across the board.  Software is leading the way from a sector perspective.  More interestingly, according to the MoneyTree report [data](https://www.pwcmoneytree.com/MTPublic/ns/moneytree/filesource/displays/notice-B.html), the gains were from expansion and later stage deals.  But by their nature, and the nature of the MoneyTree survey, early stage deals are underreported.

To dig into this trends, we can look directly at public crunchbase [data](http://info.crunchbase.com/about/crunchbase-data-exports/).

## The Numbers

<figure>
  <a href="{{ site.url }}/images/crunchbase/funding-amount-trend.png"><img src="{{ site.url }}/images/crunchbase/funding-amount-trend.png" /></a>
  <figcaption><a href="{{ site.url }}/images/crunchbase/funding-amount-trend.png" title="Amount Raised by Stage and Quarter"></a>Amount Raised by Stage and Quarter.</figcaption>
</figure>

Decomposing the total amount raised demonstrates an increasing trend across stage.  The huge increase in the quarterly amount raised is driven by companies having raised a series-C or greater.  The last quarter series-C+ dramatically increased beyond their trend.

<figure>
  <a href="{{ site.url }}/images/crunchbase/funding-trend.png"><img src="{{ site.url }}/images/crunchbase/funding-trend.png" /></a>
  <figcaption><a href="{{ site.url }}/images/crunchbase/funding-trend.png" title="Companies Funded by Stage and Quarter"></a>Companies Funded by Stage and Quarter.</figcaption>
</figure>

The number of companies that raised by quarter has very different trends by stage.  Angel and seed deals grew dramatically from 2010 through 2013 but actually decreased in the first quarter of 2014.  Anecdotally, I suspect this is due to a lag in the reporting of smaller deals and not a decline in funding.  Series A deals lagged angel deals by greater than the 9-12 months needed to raise the next round, causing the publicized Series A crunch through 2013.  Series B companies have begun an up tick but again lag earlier rounds.  Tom Tunguz demonstrates this in his post [The Hardest Round](http://tomtunguz.com/the-hardest-round-to-raise/).

Changes in capital efficiency and ease in company creation take a while to propagate through the venture economy.

## Takeaway

This increase in venture investment is being driven by investment in a handful of companies.  This is a relatively new trend of late stage pre-IPO investment from hedge funds and private equity firms.  In Q1 2014, Cloudera [raised](http://recode.net/2014/03/31/intel-takes-massive-740-million-stake-in-cloudera/) $740M from Intel, T. Rowe Price and Google Ventures.  Dropbox [raised](http://techcrunch.com/2014/02/24/dropbox-filing/) $350M from BlackRock, Morgan Stanley, T. Rowe Price. Lyft [raised](http://techcrunch.com/2014/04/02/lyft-250m/) $250M from Coatue, Alibaba, and Andreessen Horowitz. And the list continues...

This new normal of pre-IPO trend also seems to continue as Airbnb [raised](http://techcrunch.com/2014/04/18/airbnb-has-closed-its-500m-round-of-funding-at-a-10b-valuation-led-by-tpg/) $450M from TPG and T. Rowe Price in April 2014.

## Code and Data

Here is a [R script](https://gist.github.com/jdavidson/11130754) for generating graphs and see [Crunchbase](http://info.crunchbase.com/about/crunchbase-data-exports/) for the raw data.
