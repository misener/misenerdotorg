---
id: 1785
title: iTunes Smart App Banners work for podcasts, too
date: 2015-02-16T20:39:51+00:00
author: Dan Misener
layout: post
guid: http://misener.org/?p=1785
permalink: /itunes-smart-app-banners-work-podcasts/
categories:
  - Podcasting
tags:
  - iTunes
  - podcasting
---
Starting with iOS 6, Apple introduced [Smart App Banners](https://developer.apple.com/library/ios/documentation/AppleApplications/Reference/SafariWebContent/PromotingAppswithAppBanners/PromotingAppswithAppBanners.html). If you&#8217;re an iPhone person, you&#8217;ve probably seen these things at the top of mobile websites, prompting you to download a corresponding app. They link right to the iTunes app store.

I recently learned that iTunes Smart App Banners aren&#8217;t just for apps. They work for podcasts listed in the iTunes directory, and they deep link directly to the built-in Podcast app:

[<img src="http://misener.org/wp-content/uploads/2015/02/GRTTWaK_app_banner-528x139.png" alt="GRTTWaK_app_banner" width="528" height="139" class="alignnone size-medium wp-image-1786" srcset="http://home.misener.org/wordpress/wp-content/uploads/2015/02/GRTTWaK_app_banner-528x139.png 528w, http://home.misener.org/wordpress/wp-content/uploads/2015/02/GRTTWaK_app_banner.png 640w" sizes="(max-width: 528px) 100vw, 528px" />](https://itunes.apple.com/ca/podcast/grownups-read-things-they/id890900960?mt=2&uo=4&at=10lR7u)

How? Just drop this into your `&#x3C;head&#x3E;`:

`&#x3C;meta name=&#x22;apple-itunes-app&#x22; content=&#x22;app-id=XXXXXXXXX&#x22;&#x3E;<br />
` 

Where XXXXXXXXX is your iTunes podcast ID.