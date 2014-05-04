---
layout: post
title: Beyond The App Store - Mobile Discovery and Interaction
description: The next phase in mobile search and interaction is contextual deep discovery.
tags: [startup,mobile,search]
image:
  feature: discovery.png
  creditlink: http://en.wikipedia.org/wiki/File:STS-119_Discovery_landing01.jpg
share: true
---

# tl;dr The next phase in mobile search and interaction is contextual deep discovery.

Mobile discovery and interaction is still in a nascent state.  Facebook's announcement of [Applinks](http://applinks.org/) at their F8 Event and URX's [Omnilink](http://blog.urx.com/post/84368956069/omnilinks-app-links-and-the-state-of-mobile) last week sparked a ranging [conversation](https://twitter.com/pmarca/status/462475590700761088) about what both UX and technology might look like.

Mobile discovery is entering a new phase beyond just app discovery to more general engagement.  As Benedict Evans has repeatedly [argued](http://ben-evans.com/benedictevans/2014/3/18/cards-code-and-wearables), the interaction model hasn't been established for mobile.

> [O]n mobile the internet is in a pre-Pagerank phase, lacking the 'one good' discovery mechanism that the desktop web had, but it's also in a pre-Netscape phase, lacking one interaction model in the way that the web dominated the desktop internet for the last 20 years. Of course that doesn't mean there'll be one, but right now everything is wide open.

This next evolution of mobile discovery and interaction requires deep hooks into the mobile OS.  As a result, Android as a more open platform seems to be leading the way.  By allowing for advanced customization of home and lock screens, advanced context passing in Android [Intents](http://developer.android.com/guide/components/intents-filters.html), and more generally additional app store ecosystems.

Let's consider the evolution of the ecosystem.

## Phase Zero - App Stores

In July 2008, Apple launched the first version of the iOS app store with just 500 apps.  This app store was little more than a keyword search on structured meta data (title, description) provided by app developers.  Quickly, the categorized top app lists drove engagement.  This drove a rise in CPI based, incentive ad networks to propel apps up the charts.  Admob ([acquired](http://techcrunch.com/2009/11/09/google-acquires-admob/) by Google for $750M) and Tapjoy were the early players.

## Phase One - application discovery

Chomp - search algorithm improvement

The first phase of the evolution of this interaction and discovery model on top of the core mobile OS started with better search on App Stores by companies like Chomp ([acquired](http://techcrunch.com/2012/02/23/apple-chomp/) by Apple), and Quixey ([raised](http://www.crunchbase.com/organization/quixey) $75M from USVP, GGV, Alibaba).  Chomp launched in January 2009, when the iOS app store had grown to > 15,000 apps and already top 20 lists were not sufficient for app discovery.  By the time Apple acquired Chomp to improve its search algorithms in February 2012, the number of apps had grown to >500,000.

## Phase Two - contextual application discovery

Launchers and Lock / Home Screens - app organization and at a glance discovery

With both Android and iOS currently having >1M apps in their app stores, app discovery and engagement is broken.  Cover ([acquired by Twitter](http://blog.coverscreen.com/post/81998756366/cover-is-joining-twitter)), Aviate ([acquired by Yahoo](http://blog.getaviate.com/post/72586543194/aviates-going-to-get-better-faster-with-yahoo)) and 100s more launchers and smart screens organize and contextual prompt app usage.  These apps are subject to huge platform risk and is partially why these great apps needed to partner with a big platform player.  Google has already built and promoted a Google Now launcher paired with the Google search app.

The fragmented Android ecosystem has created many different forked platforms and opportunities outside the Google controlled world.  As an example, there are over 1000 app stores in China and large public Chinese companies like Sungy Mobile (the Go Launcher) [valued](http://finance.yahoo.com/q?s=GOMO) at nearly $600M.

## Phase Three - the next frontier. contextual deep discovery

Contextual deeplink search - indexing and interacting with native mobile apps

Application discovery is the first order problem.  Once you've downloaded >85 apps / device [on average](http://www.asymco.com/2013/05/31/100-billion-app-downloads/) engagement is next.  Ultimately, the UX of having to remember and find which app out of the 85 apps to interact with a given entity is unwieldy.  Exposing discovery to deeper entities is the next step.

Enter one letter and get contacts, apps and web results that are relevant just for you in your context.  Typing [L] might pull up Laura's number for Phone, or show Snapchat, SMS, Facebook Messenger to message Laura - personalized base on use and context.  Apps are the equivalent of verbs on these deeper entities.  Typing [Delfina] would pull up Delfina with options for engaging apps like Yelp for reviews, OpenTable for reservations, OrderAhead, Postmates ...

Siri - exposes some level of app and deeper discovery (but with an index that is constrained to supported Apple apps and a [rumored](http://www.forbes.com/sites/parmyolson/2014/03/05/apple-reportedly-plans-to-open-siri-to-third-parties-just-as-hackers-force-it-open/) API).  I'm also always amazed by the hidden [Spotlight Search](http://support.apple.com/kb/ht3636).  iOS has built in application search, but also surfaces a variety of entities (contacts, email, and media in iTunes).

[Google Now](http://www.google.com/landing/now/#howtogetit) - card based anticipatory search as well as Deeplink [indexing](https://developers.google.com/app-indexing/webmasters/server) and soon [ad serving](http://blogs.wsj.com/digits/2014/04/22/google-ads-will-soon-link-inside-mobile-apps/).  App discovery broadly is coming to Google apps and SERPs.

If mobile discovery follows other mobile utilities and apps, I expect we will see a disaggregation of search.  A vertical specific discovery tool allows for a more customized and optimal search experience for different use cases.  By building a mobile native app focused discovery tool, there is an opportunity to build a better search experience than Google's browser based and web biased search.  I expect it will organize by entity.

Entities:

* People - Smart contact managers are starting to pop up to allow for contact across multiple communication apps.
* Places - The Yelp platform allows users to discover a place to see user reviews from their platform but also to book on OpenTable, order delivery via Eat24 and so on.
* Media - I'd argue there is no great multi-media search tool but YouTube for mobile has near ubiquitous coverage.
* Things (Product) - Like media this isn't quite there.  Amazon for mobile has near ubiquitous coverage.

This fragmentation is the case in other utilities and will likely happen across search.

Communication apps have proliferated due to the ease of contact import.  Each app has a specific use case and unique circle.  There are some people I text, some I exclusively talk to on GroupMe, some use SnapChat ...  This has started.

Similarly, a suite of local business service apps are emerging.  DoorDash, PostMates and [soon](http://blog.uber.com/RUSH) Uber cover delivery, OpenTable and SeatMe create reservations, Yelp and Foursquare facilitate discovery and comparison.  When I search for a place, a variety of apps now provide the information or action I might need.  Instead of Google just surfacing the choice between Yelp for reviews or OpenTable to make a reservation, mobile search needs to be able to contextually request immediate delivery or reservation or purchase knowing where I am and what I like.

# The next Google?

These new interaction models will also allow for new promotional business models.  Beyond just [re-targeting and re-engagement]({{ site.url }}/mobile-engagement/), as Google has shown on the web, influencing discovery and harnessing intent is very valuable.  The company that gets discovery right can be thought of as the mobile Google.   There will naturally be a mobile Adwords as well.

As the web and desktop computing did previously.  The transition to a mobile first and in many cases only platform allows for the possible reinvention of existing technology business models.  In this, Google's ownership of Android is clearly beneficial but I don't think is necessarily a prohibitive advantage.  The ability of a startup focusing on a small but growing market has time and again beaten larger incumbents.  I look forward to the innovation!

