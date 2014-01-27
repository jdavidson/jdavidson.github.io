---
layout: post
title: Apple Q4 2013 Earnings Prediction using Google Trends
description: Google trends indicate soft quarter for iPhone sales
tags: [data, apple]
share: true
---

# tl;dr Google trends indicate soft quarter for iPhone sales

Apple earnings are a bellwether for the technology industry and the iPhone has become Apple’s most important product, accounting for more than half of its revenue.  In advance of their reporting today, I thought it would be fun to take a page from Hal Varian's [Predicting the Present](http://static.googleusercontent.com/media/www.google.com/en/us/googleblogs/pdfs/google_predicting_the_present.pdf), and run a quick, non-scientific stab at predicting iPhone sales based on [Google query traffic](http://www.google.com/trends/explore#q=iphone).

<figure>
  <a href="http://www.google.com/trends/explore#q=iphone"><img src="{{ site.url }}/images/iphone-queries.png" /></a>
  <figcaption><a href="{{ site.url }}/images/iphone-queries.png" title="Google query traffic trends for iPhone">Google query traffic trends for [iPhone]</a></figcaption>
</figure>


Overlaying normalized iPhone quarterly sales demonstrates a very strong relationship (a correlation of >.75).

<figure>
  <a href="{{ site.url }}/images/iphone-norm-sales-queries.png"><img src="{{ site.url }}/images/iphone-norm-sales-queries.png" /></a>
  <figcaption><a href="{{ site.url }}/images/iphone-norm-sales-queries.png" title="Normalized Apple iPhone Sales and Google Search Query Index">Normalized Apple iPhone Sales and Google Search Query Index.</a></figcaption>
</figure>

With [estimates](http://blogs.wsj.com/digits/2014/01/27/apple-earnings-what-to-watch-2/) in the >50M units range based on the strength of the newly released iPhone 5c and 5s, Apple is expected to have a monster quarter.  A trivially simple linear model from Google search trends yields a much softer prediction for Q4 2013, on the assumption that Google query traffic is causally related to purchase intent and thus actual sales.  Note, this is certainly woefully unsophisticated.

<figure>
  <a href="{{ site.url }}/images/iphone-pred-sales.png"><img src="{{ site.url }}/images/iphone-pred-sales.png" /></a>
  <figcaption><a href="{{ site.url }}/images/iphone-pred-sales.png" title="Apple iPhone Sales and Q4 2013 Prediction">Apple iPhone Sales and Q4 2013 Prediction</a></figcaption>
</figure>

Soft query volume on iPhone may indicate a soft Apple quarter.

# Caveat!

Naturally, this blog would never imply that correlation equals causation.  While Hal has repeated demonstrated the accuracy of using Google query traffic, tapping "database of intentions" as John Batelle has called it, this is a trivial analysis for fun.

Or as Facebook's Mike Develin said in a great [response](https://www.prod.facebook.com/notes/mike-develin/debunking-princeton/10151947421191849) to the recent Princeton researchers [paper](http://arxiv.org/pdf/1401.4208v1.pdf) applying a similar methodology drawing a conclusion about Facebook from Google Trends:
>> As data scientists, we wanted to give a fun reminder that not all research is created equal – and some methods of analysis lead to pretty crazy conclusions.


## Code and Data

Here is a [R script](https://gist.github.com/jdavidson/8654897) for generating graphs and see [Statista](http://www.statista.com/statistics/263401/global-apple-iphone-sales-since-3rd-quarter-2007/) and [Google Trends](http://www.google.com/trends/explore#q=iphone) for the raw data.

