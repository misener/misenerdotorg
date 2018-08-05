---
id: 243
title: Scheduled syncing with iSync
date: 2007-02-26T08:30:51+00:00
author: Dan Misener
layout: post
guid: http://www.danmisener.com/archives/243
permalink: /scheduled-syncing-with-isync/
categories:
  - phones
  - Software
---
<img align="right" title="iSync logo" alt="iSync logo" src="http://images.apple.com/macosx/features/isync/images/indextop20050412.jpg" />I like my cell phone (a [Motorola L7](http://www.motorola.com/motoinfo/product/details.jsp?globalObjectId=86)) just fine. It&#8217;s small-ish, the speaker volume is sufficient, and through iSync, it can keep in touch with my address book and calendar using Bluetooth.

Problem is, I never remember to actually sync the darned thing, so the information on my phone is always hopelessly out of date. So I&#8217;ve come up with a solution &#8212; scheduled syncing:

  1. I copied Fraser Speirs&#8217;s [Synchronize with iSync, then Quit](http://speirs.org/wiki/Scripts#Synchronize_with_iSync.2C_then_Quit) script into Script Editor, then saved it as an application.
  2. Then I set up a cron job to periodically run the script. I used [CronniX](http://www.abstracture.de/projects-en/cronnix) to do this, because I&#8217;m no Unix geek.

The result? When my computer is on, and my phone is within range, it&#8217;s periodically synchronized with iCal and Address Book. If my phone is out of range, it fails and quits iSync.