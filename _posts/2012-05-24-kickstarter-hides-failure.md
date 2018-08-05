---
id: 1354
title: Kickstarter hides failure
date: 2012-05-24T08:50:13+00:00
author: Dan Misener
layout: post
guid: http://misener.org/?p=1354
permalink: /kickstarter-hides-failure/
categories:
  - internet
tags:
  - crowdfunding
  - failed projects
  - kickstarter
  - scraping
  - scrapy
---
(**TL;DR:** Kickstarter does not want you to see failed projects. Failed Kickstarter campaign pages include robot meta tags to keep search engines from indexing them. Plus, Kickstarter&#8217;s front page and &#8220;Discover&#8221; interface never show failed projects. Ever.)

**Update @ 17:30 CET:** In response to some great feedback over at [Hacker News](http://news.ycombinator.com/item?id=4018393), I&#8217;ve made a few edits below to clarify a few points. First, to emphasise that failed results _do_ show up in Kickstarter&#8217;s own search results. Second, to clarify that I don&#8217;t think there&#8217;s anything nefarious or ill-intentioned going on here. Just that Kickstarter has made an interesting design decision when it comes to how it displays (or doesn&#8217;t display) &#8220;failed&#8221; projects.

&#8212;

## Only show success

Here&#8217;s a fun crowdfunding experiment: visit [Kickstarter&#8217;s main page](http://www.kickstarter.com/), click around, and without using the search box, try to find a project that isn&#8217;t either:

**a)** Successful
  
**b)** In progress

You can&#8217;t.

Spend more than a few minutes poking around, and you&#8217;ll realize that Kickstarter&#8217;s front page and Discover pages are clearly built to highlight projects that are currently seeking funding, or have already been successfully funded.

From a business perspective, this makes total sense. Kickstarter&#8217;s business model is built on taking a 5% cut of successful campaigns. Showing failures isn&#8217;t in their interest.

First, failed projects aren&#8217;t actionable. No one can back a project that&#8217;s already missed its funding goal.

Second, failed projects look bad. If you&#8217;re trying to convince the world that anyone can crowdfund anything, it doesn&#8217;t help to remind people that 56% of Kickstarter projects fail to meet their funding goal.

When I first noticed that Kickstarter&#8217;s web interface wasn&#8217;t showing me any failures, I wanted to be sure. To confirm my suspicions, I wrote a scraper (using the excellent [Scrapy framework](http://scrapy.org/)) designed to browse through Kickstarter&#8217;s [Discover](http://www.kickstarter.com/discover) pages, extracting project details from every single campaign page it could find.

The result: [27,399 projects](https://www.google.com/fusiontables/DataSource?docid=15dxZcTzOdu1QyLBoF1DDd2o3ZErWxeHSUOmxWIo)[1. Of the 27,399 projects I scraped, 23,059 were successful, and 4,340 were in progress. Given that the New York Times [recently reported](https://www.nytimes.com/interactive/2012/04/30/technology/three-years-of-kickstarter-projects.html) that there are about 50,000 projects on Kickstarter, and given Kickstarter&#8217;s widely cited 44% overall success rate, 23,059 successful projects suggests that my scraper got _all_ the successful projects.]. Every single project my scraper could find was either successful or in progress.

This means that if you&#8217;re a human being (instead of a scraper) you could browse Kickstarter&#8217;s Discovery section for days, weeks, or months. You could look at more than 27,000 projects. And you&#8217;d never come across a failure.

## Hide failed projects from Google

To be clear, Kickstarter doesn&#8217;t pull failed projects off their site.

Links to failed Kickstarter projects still work. For example, I can still link to [Instaprint](http://www.kickstarter.com/projects/breakfastny/instaprint-the-location-based-photo-booth-for-inst), a project that failed to meet its funding goal on April 29. Or, if you know the name of a failed project, you can search for it using Kickstarter&#8217;s search engine. Here&#8217;s [a search for Instaprint](http://www.kickstarter.com/projects/search?term=Instaprint). The project also shows up in the [search results for &#8220;instagram&#8221;](http://www.kickstarter.com/projects/search?term=instagram) and &#8220;[photo booth](http://www.kickstarter.com/projects/search?term=photo%20booth)&#8220;.

But here&#8217;s the thing: search for Instaprint on [Google](https://encrypted.google.com/search?hl=en&q=instaprint), or [Bing](http://www.bing.com/search?q=instaprint), or [DuckDuckGo](https://duckduckgo.com/?q=instaprint), and the Kickstarter project page is nowhere in the results.

Why?

In the header section of every single failed Kickstarter project I could find, I found this [robots meta tag](http://www.robotstxt.org/meta.html):

    <meta name="robots" content="noindex"/>

This tag, which shows up on failed Kickstarter projects, but not on successful or in progress projects, tells search engines to ignore the page.

Kickstarter doesn&#8217;t pull failures off their site. They just make it difficult to find them through third-party search engines.

## So what?

I don&#8217;t think Kickstarter is doing anything nefarious or ill-intentioned here. It makes perfect business sense for them to keep their main page and discovery mechanism free of failed projects.

I point this out because Kickstarter has made an interesting design decision.

Mostly, I find Kickstarter&#8217;s approach an interesting counterpoint to other types of online transaction platforms. eBay, for example, displays auctions that weren&#8217;t successful (you can even search for them). When an item is out of stock on Amazon, you can still search for it.

Kickstarter&#8217;s &#8220;hide failures&#8221; tactic is also interesting when compared to other crowdfunding sites. For example, Indiegogo seems to list unsuccessful projects[2. Yes, I understand that the definition of &#8220;successful&#8221; is different on Indiegogo than Kickstarter. Some projects that don&#8217;t meet their their funding goals still receive money.] alongside successful ones.

But mostly, I think this matters for entrepreneurs who are planning to use Kickstarter as a funding platform. Recently, I talked to Scott Steinberg, who wrote [The Crowdfunding Bible](http://www.crowdfundingguides.com/), and he talked about why research is so important for entrepreneurs.

He told me that if you&#8217;re going to use a crowdfunding service like Kickstarter, it&#8217;s important to figure out what&#8217;s worked for others in the past, but also to figure out _what hasn&#8217;t worked for others in the past_.

If you hide failure, it&#8217;s hard to learn from others&#8217; mistakes.