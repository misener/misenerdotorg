---
id: 429
title: 'You can&#8217;t block users from private Meraki mesh networks'
date: 2009-01-31T12:51:13+00:00
author: Dan Misener
layout: post
guid: http://danmisener.com/archives/429
permalink: /you-cant-block-users-from-private-meraki-mesh-networks/
categories:
  - meraki
  - wifi
tags:
  - meraki
  - mesh network
  - wifi
---
If someone knows the WPA2 password to your Meraki mesh network, and you want to block them, you can&#8217;t. The block function only works on the public network. Meraki&#8217;s Jeff Gould explains in an email to me:

> The blocking function works only on the public network. There is no blocking capacity on the private Meraki Network. There are a variety of folks who would like to have this functionality and I believe that we will have features to address this in 2009.

Wow. So, like, sometime this year? That&#8217;s kind of vague.

Right now, it seems the only way to keep someone that knows your password off your network is to change your password.