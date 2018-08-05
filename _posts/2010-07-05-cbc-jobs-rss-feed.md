---
id: 644
title: CBC Jobs RSS feed
date: 2010-07-05T16:07:23+00:00
author: Dan Misener
layout: post
guid: http://misener.org/?p=644
permalink: /cbc-jobs-rss-feed/
categories:
  - CBC
tags:
  - CBC
  - jobs
  - taleo
---
**Update June 7, 2011:** MediaJobsSearchCanada&#8217;s RSS feed no longer includes 8-character CBC job numbers (e.g. EDM00183), which breaks the whole thing I&#8217;d rigged up in Yahoo Pipes. I may someday write my own scraper for CBC&#8217;s terrible jobs site, but until then, the feed won&#8217;t be updated. Curiously, the MJSC change seems to have happened _one day_ after CBC HR took control of @CBCjobs. Coincidence?

**Update May 19, 2011:** A representative from CBC HR asked for control of the @CBCjobs Twitter handle. I agreed to change the Twitter username of my automated CBC job posting robot, allowing them to create a new account with the @CBCjobs username. It appears that they&#8217;ve created a new account under the name @CBCjobs, listing it as the &#8220;Official account for HR @ Canada&#8217;s national public broadcaster.&#8221; As I write this, the account seems to be manually updated, _without_ automatic job postings. Too bad.

If you still want automated CBC jobs postings, you can now follow [@workatCBC](https://twitter.com/#!/workatCBC) on Twitter, or subscribe to this feed: <http://feeds.feedburner.com/workatCBC>. If you were previously following @CBCjobs, Twitter should have automatically switched you over.

===

Here&#8217;s the short version of this story: The [CBC&#8217;s jobs website](http://cbc.ca/jobs/) doesn&#8217;t have an RSS feed. So I made one:

<p style="padding-left: 30px;">
  <del datetime="2011-05-20T02:40:05+00:00"><a href="http://feeds.feedburner.com/cbcjobs">http://feeds.feedburner.com/cbcjobs</a></del>
</p>

<p style="padding-left: 30px;">
  <a href="http://feeds.feedburner.com/workatCBC">http://feeds.feedburner.com/workatCBC</a>
</p>

This feed is completely unofficial, and comes with no guarantees. You can also follow [<del datetime="2011-05-20T02:40:05+00:00">@cbcjobs</del> @workatCBC on Twitter](http://twitter.com/workatCBC) if you&#8217;re into that sort of thing.

You&#8217;re welcome.

&#8212;

Here&#8217;s the longer version of the story: The CBC&#8217;s jobs website (&#8220;Powered by [Taleo](http://www.taleo.com/)&#8220;) is basically pretty terrible. And astonishingly, it doesn&#8217;t have an RSS feed. If you want new CBC job postings via RSS, you can get them from a couple of places, but these sources aren&#8217;t exactly what I was looking for:

  * [The Tea Makers HR Department](http://www.theteamakers.com/author/tmhr/feed/) (appears to be a human-powered cut/paste job, sometimes delayed by days)
  * [CBCJobsBC on Twitter](http://twitter.com/CBCJobsBC) (seemingly official, but only posts jobs in British Columbia)
  * [MediaJobSearchCanada&#8217;s main RSS feed](http://feeds.feedburner.com/MediaJobSearchCanadaJobs) (updated frequently &#8211; by a scraper, I suspect, but contains every media job in Canada, and links point back to MJSC, where you can&#8217;t directly apply for any jobs)

So, using Yahoo Pipes and Feedburner, I cobbled together a feed that I hope will be useful to some people. Basically, [this pipe](http://pipes.yahoo.com/misener/cbcjobs) takes the frequently-updated MJSC feed, and then filters out postings that don&#8217;t have &#8220;CBC RADIO-CANADA&#8221; listed as the Company. Then, it grabs the 8-character CBC job number (e.g. EDM00183) from the title, and appends it to

<pre>https://cbc.taleo.net/careersection/2/jobdetail.ftl?job=</pre>

to create a permalink. Feedburner makes the feed pretty, and periodically sends new postings to [<del datetime="2011-05-20T02:40:05+00:00">@cbcjobs</del> @workatCBC on Twitter](http://twitter.com/workatcbc).

Obviously, it would be much better if the CBC made official job RSS feeds available, but until then, I hope this helps some people out.