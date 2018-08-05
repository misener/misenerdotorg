---
id: 620
title: Pie charts are terrible
date: 2010-02-12T09:46:46+00:00
author: Dan Misener
layout: post
guid: http://misener.org/?p=620
permalink: /pie-charts-are-terrible/
categories:
  - Uncategorized
---
Yesterday, Google [announced](http://googlecode.blogspot.com/2010/02/announcing-google-chart-tools.html) [Google Chart Tools](http://code.google.com/apis/chart/image_charts.html), reminding us that:

> A good chart can take an elusive concept and clarify it in a visually appealing manner.

It&#8217;s pretty cool. You can dynamically generate charts using URLs. Their example turns this:

`http://chart.apis.google.com/chart?cht=p3&chd=t:60,40&chs=250x100&chl=Hello|World`

into a [pie chart](http://code.google.com/apis/chart/docs/gallery/pie_charts.html):

![](http://chart.apis.google.com/chart?cht=p3&chd=t:60,40&chs=250x100&chl=Hello|World)

While this \_is\_ pretty slick (and Google&#8217;s service generates many, many types of charts), I think this is as good a time as any to remember that [pie charts are terrible](http://seedmagazine.com/content/article/getting_past_the_pie_chart). SEED magazine summarizes findings from [Bill Cleveland](http://www.stat.purdue.edu/~wsc/) (emphasis mine):

> although we’re good at comparing linear distances along a scale — judging which of two lines is longer, a task used in bar graphs — and we’re even better at judging the position of points along a scale, pie charts don’t bring those skills to bear. They do ask us compare angles, but we tend to underestimate acute angles, overestimate obtuse angles, and take horizontally bisected angles as much larger than their vertical counterparts. The problems worsen when we’re asked to judge area and volume: **Regular as clockwork, we overestimate the size of smaller objects and underestimate the size of larger ones, to a much greater degree with volume than with area.**

**Update (15 April 2011):** Via [Nora Young](http://norayoung.ca/), a link to new evidence that [pie charts aren&#8217;t as bad as some people believe](http://eagereyes.org/criticism/in-defense-of-pie-charts).