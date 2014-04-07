---
layout: post
title: Flywheel - building to marketplace liquidity
description: Marketplaces = liquidity.  Simplify and cheat as much as possible to get started.
tags: [marketplace,startup,econ]
image:
  feature: flywheel.jpg
  creditlink: http://commons.wikimedia.org/wiki/File:Water_wheel_at_the_Wellbrook_Beetling_Mill_(Cookstown).jpeg
share: true
---

# tl;dr Marketplaces = liquidity.  Simplify and cheat as much as possible to get started.

Steve Schlaf's has an excellent [overview](http://schlaf.me/post/81679927670) of the on-demand mobile services.  Many, if not all, of these services represent modern evolutions of service marketplaces.  This isn't surprising, marketplaces from eBay to Kickstarter to Uber are a triumph of the power of the internet and now mobile computing.  Goods and services that previously didn't have sufficient demand in local markets can now market to the globe.  Services ticking Bill Gurley's [10 Factors for a digital marketplace](http://abovethecrowd.com/2012/11/13/all-markets-are-not-created-equal-10-factors-to-consider-when-evaluating-digital-marketplaces/), large markets with high fragmentation, poor experiences, economic burden and network effects, can be rethought.

Schlaf's map is partially representative of Andrew Parker's earlier [unbundling of Craiglist](http://thegongshow.tumblr.com/post/345941486/the-spawn-of-craigslist-like-most-vcs-that-focus).  The surprise isn't that Craigslist is disaggregating, it's that it is taking so long (note Andrew's piece was written at the beginning of 2010).  A marketplace that reaches liquidity is difficult to unseat even as poor an experience and diverse as Craiglist.

The proliferation of these service marketplaces reflects the value they have at liquidity.  The lack of speed of this disaggregation reflects the incredible difficulty in reaching that liquidity.  These two sided marketplaces have the classic [chicken-and-egg](http://en.wikipedia.org/wiki/Chicken_or_the_egg) cold-start problem.

As a quick background, I've spent most of my career focused on various marketplaces: Ad - Google, Media - YouTube, Local - PrimaTable, and most recently Travel - Hotel Tonight.

# Two Sided Marketplace

A two sided marketplace requires both buyers and sellers.  Buyers are only interested in relatively valuable supply and vice versa.

To be successful, two sided marketplaces must build essentially two businesses.  Uber must sell drivers on the value of their market relative to their other options through price, liquidity, aggregated demand and services like payments and insurance.  At the same time, they also create a great customer experience and user acquisition through P&R, mobile user acquisition, and virality.

At scale, everything needs to be automated to facilitate liquidity.  Until you get there manually faking the market can get the flywheel going.  Let's consider both sides of the market.

# Supply and Demand

Faking the seller (supply) side of the market is often the easiest.  For a seller, a new marketplace represents integrating a new channel for the possibility to make more money.  In service marketplaces, this new channel is often exclusive and thus the risk associated requires a commensurate economic incentive in the form of relative value.  Suppliers primarily care about liquidity - defined by [wikipedia](http://en.wikipedia.org/wiki/Market_liquidity) as "a market's ability to facilitate an asset being sold quickly".

Demand can be harder to build and requires ubiquity of coverage and quality of supply to enable trust in the market.  This ubiquity and quality drive toward increased liquidity.  Growing one side of a market offers increased value to the other due to [network effects](http://en.wikipedia.org/wiki/Network_effect).

### 1. Single side utility
OpenTable [built](http://www.quora.com/How-did-OpenTable-form-its-first-partnerships-with-restaurants) two different products with different value propositions.  For top restaurants, not needing help generating demand, they built a CRM service to allow them to better services customers.  The next tier of restaurants, aspiring to the top, joined valuing an increased demand.
Google built a better search product, syndicated their service and aggregated user demand before offering a CPC ad model.[^1]

### 2. Integrations
AirBnB [famously](http://www.quora.com/Did-Airbnb-really-need-to-illegally-spam-on-Craigslist-in-order-to-build-a-market) solicited existing Craiglist suppliers.  By leveraging other channel listings (often eBay or Craiglist), a marketplace can have comprehensive coverage of supply and without a direct relationship with all suppliers.

### 3. Focus
Yelp focused on geography (SF) and vertical (restaurants), while actively recruiting power users, deriving value from participation, prior achieving utility to a broader set of users for local discovery.  By limiting the market from all local search to primarily focusing on SF restaurants, Yelp was able to get to a critical mass and thus utility.  They drove toward saturation and liquidity in their local market.  Local discovery in particular is hard to get to ubiquity due to the sparsity of coverage as highlighted by Pat Kinsel's recent [post on the problem with local search](http://patkinsel.com/post/81293994011/the-problem-with-local-search-and-discovery).  A network requires critical mass of coverage.

### 4. Inventory
By explicitly purchasing inventory, marketplaces can generate an initial amount of supply.  [Rolling out](http://www.quora.com/Uber-1/In-the-first-1-000-days-of-Uber-what-was-the-strategy-for-solving-the-chicken-egg-problem-of-building-out-a-two-sided-marketplace-How-much-of-the-process-was-manual-i-e-calling-drivers-vs-automated-i-e-GPS-location-based) Uber in a new market requires hiring drivers at an hourly rate to attract customers to the valuable option.  This is often subsidized but can represent an arbitrage opportunity.  This is not intended to last and is different than one sided ecommerce businesses, like Amazon, where the model is to be the merchant of record and resell merchandise.

### 5. Syndication
YouTube used MySpace embeds for both user acquisition and for broader media distribution.  Early users derived value from uploading content to YouTube both on the YouTube platform and gaining initial distribution through embeds on existing channels.

### 6. Scarcity
A story about YouTube wouldn't be complete without looking at their use of the [DMCA](http://www.quora.com/YouTube/How-did-YouTube-gain-its-initial-traction).  By adopting a relatively liberal view (and ultimately vindicated) of the DMCA, YouTube often had exclusive infringing content like rips of the Colbert Report and SNL.  In markets where demand exceeds supply (e.g. collectibles, antiques, luxury products) – two sided marketplace problem can be solved by focusing on the in demand scarce inventory.

### 7. Manual
This is an extension of Paul Graham's ["Do things that don't scale"](http://paulgraham.com/ds.html).  In time vs money, delivery start ups like Postmates, [offering](http://www.fastcompany.com/3000883/what-apps-upper-class-mean-99) broad local business coverage with explicit relationships can be prohibitively difficult.  By manually fulfilling user demand, Postmates will offer menus at uncovered merchants and send a courier to order like a normal customer.  The network is able to offer better coverage than otherwise possible, driving like all others to ubiquity and liquidity.


[^1] Similar to social networks covered in Andrew Chen's fantastic [post](http://andrewchen.co/2014/03/27/how-to-solve-the-cold-start-problem-for-social-products/)