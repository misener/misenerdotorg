---
id: 1821
title: How many top podcasts use SSL feeds?
date: 2016-09-29T11:05:59+00:00
author: Dan Misener
layout: post
guid: http://misener.org/?p=1821
permalink: /how-many-top-podcasts-use-ssl-feeds/
categories:
  - Podcasting
---
In early 2016, Apple [added support for SSL-secured podcast feeds](http://itunespartner.apple.com/en/podcasts/news/56206386).[^1]

I wanted to get a sense of how many shows are taking advantage of this, so I grabbed a [list of the top 200 podcasts in iTunes (US), along with their feed URLs](https://docs.google.com/spreadsheets/d/1aD7D3J0D7jbHhAdDDv9t66WsZMXga0gaRQdZ0G3ay00/edit?usp=sharing).

A few observations:

  * **Only 11 of the top 200 shows (5.5%) use HTTPS for their podcast XML.** The remaining 189 feeds use plain old HTTP.
  * [Libsyn](https://www.libsyn.com/) seems to offer HTTPS versions of all its podcast feeds, but _none_ of the 34 Libsyn-hosted podcast feeds on the iTunes US Top 200 use the SSL-secured version.
  * [Art19](http://art19.com/) also seems to offer HTTPS versions of its podcast feeds, but only a few (_Sword and Scale_ and _The Vanished Podcast_) in the Top 200 use them.
  * All [Audioboom](https://audioboom.com/)-hosted feeds listed in the US iTunes Top 200 (_Undisclosed_, _Savage Nation with Michael Savage_, _The Night Time Podcast_, _Actual Innocence_, _SpyCast_) use HTTPS.

Of course, many of the shows on the iTunes Top 200 predate Apple’s support for SSL-secured podcast feeds.

It’ll be interesting to see if more high-ranking shows make the switch to secure feeds in the coming months.

If your podcast host supports HTTPS feeds, you can (and probably should) update your feed URL using [Apple’s Podcasts Connect](https://podcastsconnect.apple.com/) and the [itunes:new-feed-url](https://help.apple.com/itc/podcasts_connect/?lang=en#/itca489031e0) feed element.

[^1]: Though some people 
    [seem miffed](https://community.letsencrypt.org/t/itunes-rejecting-le-certs/11486) that [Apple&#8217;s list of approved certificate providers](http://itunespartner.apple.com/en/podcasts/news/19855810) doesn’t include [Let’s Encrypt](https://letsencrypt.org).