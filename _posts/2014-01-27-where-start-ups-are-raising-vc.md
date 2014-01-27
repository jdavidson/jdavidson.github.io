---
layout: post
title: San Francisco is the new center of start up activity
description: The geographic distribution of capital raised is changing rapidly.
tags: [data, vc, crunchbase]
share: true
---

# tl;dr Start up fund raising is growing across the board and increasing in geographic diversity.

The new year presents a great opportunity to look back at trends in start up activity and fund raising.  [Pitchbook](http://pitchbook.com/2014_Annual_US_VC_Valuations_and_Trends_Report.html) has created a great summarization of start up funding and valuations from 2013.

<figure>
  <a href="http://pitchbook.com/2014_Annual_US_VC_Valuations_and_Trends_Report.html"><img src="{{ site.url }}/images/crunchbase/raised trend.png" /></a>
</figure>

We can see that aggregate dollars raised in 2013 is up slightly from 2012 but both down for the peak in 2011.  Let's examine geographic dispersion to better understand and visualize the broader trend.  Thanks to [Crunchbase's](http://info.crunchbase.com/about/crunchbase-data-exports/) open platform and [Google](https://developers.google.com/maps/documentation/geocoding/)'s geocoding, there is raw data to analyze.

## The Maps

<figure>
  <a href="{{ site.url }}/images/crunchbase/raised-2013.png"><img src="{{ site.url }}/images/crunchbase/raised-2013.png" /></a>
  <figcaption><a href="{{ site.url }}/images/crunchbase/raised-2013.png" title="Venture capital raised in 2013, by US Region"></a>Venture capital raised in 2013, by US Region.</figcaption>
</figure>

As also reported by [CB Insights](http://www.cbinsights.com/blog/trends/venture-capital-report-2013), California dominates start up funding with New York and Boston closely following.  This static view of the distribution of fund raising activity doesn't present the full picture.  Inspired by a beautiful Foursquare [visualization](https://foursquare.com/infographics/pulse#san-francisco), where check ins represent the heart beat of a city, I've taken a pass at representing the heart beat of the US economy through start up activity.

### Some GIFs

<figure>
  <a href="{{ site.url }}/images/crunchbase/raised-year.gif"><img src="{{ site.url }}/images/crunchbase/raised-year.gif" /></a>
  <figcaption><a href="{{ site.url }}/images/crunchbase/raised-year.gif" title="Venture capital raised, by US Region"></a>Venture capital raised, by US Region. Each frame is one year.</figcaption>
</figure>

In the animated gif above, each frame is the funding data for one year starting in 2005 through 2013.  2005, investment is mainly centered in NY, SF and Boston with little start up activity in more diverse areas.  These central tech hubs see large gains over the 8 years covered. As the decade progresses, the start up community begin to also grow in Dallas, Austin, Raleigh NC, Seattle, DC, Chicago and beyond.  Some of these secondary cities have now grown beyond where NY and Boston started.  In a network effect business, which I would argue  includes technology start ups, solving the chicken and egg problem is the most difficult.  Now that technology start ups have passed a reasonable scale in the top 10 US cities, we can hope that the pace of innovation will continue to accelerate.  There are benefits to starting a company in Silicon Valley but the success of some large unicorns outside of the bay area proves it is not a requirement (this is a big enough topic to warrant an independent post).

<figure>
  <a href="{{ site.url }}/images/crunchbase/ca-raised-year.gif"><img src="{{ site.url }}/images/crunchbase/ca-raised-year.gif" /></a>
  <figcaption><a href="{{ site.url }}/images/crunchbase/ca-raised-year.gif" title="Venture capital raised, by CA City"></a>Venture capital raised, by CA City. Each frame is one year.</figcaption>
</figure>

In the more mature tech market of California, the center of gravity has moved north from silicon valley to San Francisco proper.  In the mid aughts, Silicon Valley and San Jose represented the majority of the Bay Area investment.  As the teens turn, San Francisco became the focal point for start up activity.  We also see that LA and San Diego have continued to grow in terms of raw investment dollars.  I expect with the recent sale of a company like [Gravity](http://www.nytimes.com/2014/01/24/business/media/aol-buys-gravity-a-firm-that-personalizes-web-searches.html)[^1] that the LA area will continue to see new investment.

<figure>
  <a href="{{ site.url }}/images/crunchbase/sf-raised-year.gif"><img src="{{ site.url }}/images/crunchbase/sf-raised-year.gif" /></a>
  <figcaption><a href="{{ site.url }}/images/crunchbase/sf-raised-year.gif" title="Venture capital raised, in SF Bay Area"></a>Venture capital raised, in SF Bay Area. Each frame is one year.</figcaption>
</figure>

Zooming into the Bay Area, we see that aggregate dollars raised is increasing and spreading out.  The center of gravity has become San Francisco.  The bay area, like the US and CA, sees increased geographic distribution.  There has been increased investment beyond Palo Alto distributed across communities like Berkeley, Mountain View, Fremont and San Jose.

## Takeaway

Start up fund raising is growing across the board and increasing in geographic diversity.  In new start up empire, all roads lead to San Francisco.

## Code and Data

Here is a [R script](https://gist.github.com/jdavidson/8591371) for generating graphs and see [Crunchbase](http://info.crunchbase.com/about/crunchbase-data-exports/) for the raw data.

[^1]: Redpoint portfolio company.
