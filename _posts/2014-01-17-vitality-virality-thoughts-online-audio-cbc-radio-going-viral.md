---
id: 1690
title: 'Vitality, not virality (or, a Few Thoughts About Online Audio, CBC Radio, and &#8220;Going Viral&#8221;)'
date: 2014-01-17T00:45:31+00:00
author: Dan Misener
layout: post
guid: http://misener.org/?p=1690
permalink: /vitality-virality-thoughts-online-audio-cbc-radio-going-viral/
process_flickr_shortcode:
  - "0"
categories:
  - Public Radio
---
If you work in or care about public radio, podcasting, or online audio, I _strongly_ recommend Stan Alcorn&#8217;s terrific piece [Is This Thing On? Why Audio Never Goes Viral](http://digg.com/originals/why-audio-never-goes-viral).

In it, Alcorn digs into some of the reasons audio is a second-class citizen online: the web is a primarily visual medium, audio content is difficult to index, search, and skim through, etc.

But he also drops some telling data points about just how non-viral audio really is. For instance (emphasis mine):

> In June 2013, the list of the 100 most-shared news articles on Facebook included three from NPR, but **none included audio**.

And this:

> “Radiolab” and “This American Life” — public radio shows that are among the most popular podcasts and the aesthetic guiding lights for young public radio producers — are both approaching a million digital listens for each new episode. For these shows, the occasional episode will get shared more than others, but **that “viral” bump is on the order of 10 to 20 percent, and even that seems driven less by social media than old-fashioned word of mouth.**

Needless to say, Alcorn got me thinking a lot about the way we approach online audio and social media at CBC Radio, which at the moment seems to be placing an increasing level of importance on online metrics like pageviews and audio streaming.

If virality is indeed a worthy goal for a public broadcaster (and I&#8217;m not convinced it is, but more on that later), what are some things that CBC Radio could do to help make that happen? If we want more of what we do to (pause for cringe) &#8220;go viral,&#8221; how do we create the best possible conditions for that to happen?

Here are a few thoughts.

# More pupose-built audio tools

When CBC Radio producers make radio shows, we use tools purpose-built for audio. In studio, we use pro-level audio gear. We mix and edit sound using software built [specifically for radio](http://www.dalet.com/radio-suite).

But online, we use tools that were _never really intended for audio_.

Most CBC Radio websites run on [a blogging engine built for text](http://movabletype.org/ ".">a CDN</a> that desc"). Our audio content lives at [a CDN](http://theplatform.com/ "online video platform.") that describes itself as an &#8220;online video platform.&#8221;

Should we be surprised when tools built for sharing text and video don&#8217;t work particularly well for a completely different medium with its own set of strengths, weaknesses, and modalities?

If you want me to mash potatoes, don&#8217;t hand me a whisk.

So then, it comes as absolutely no suprise when Alcorn writes, &#8220;If there is any company attempting to create a modern web alternative to the podcast, it’s SoundCloud.&#8221;

Why? Because SoundCloud was built from the ground up to be an audio platform.

Speaking of tools&#8230;

# Build audio players with sharing and spreadability in mind

The existing embedded CBC audio players are terrible. I&#8217;d embed one here, but I don&#8217;t want to put you through that. How terrible are these players? Let me count the ways:

They&#8217;re built in Flash. They don&#8217;t work on iOS. You can&#8217;t embed them on Facebook. By default, they auto-play. They&#8217;re wasteful, because they start downloading and playing an audio file regardless of whether the user clicks play or not. They don&#8217;t link back nicely to related non-audio content. And finally, the CBC has an agressive expiration policy for archived audio. The player enforces this, even if the underlying audio is still available.

[Luc Latulippe summed it up nicely](http://blog.drawn.ca/post/26632379737/yesterday-on-cbcs-q-jian-ghomeshi-interviewed):

> Trying to embed the CBC’s audio player is like trying to nail Jell-O to a tree

Public broadcasters can&#8217;t realistically expect listeners to share and spread radio stories if the experience of doing so is absolultely miserable.

# Slice it up

As I wrote back in 2011, [segmentation matters](http://misener.org/segmentation-matters/):

> People want what they want when they want it. Offering easy access to individual stories (like TAL does, or how Quirks and Quarks offers a segmented podcast) helps people share and spread the stories they love. It helps create the conditions for virality.

Things **are** getting better at the CBC. We&#8217;re slicing up audio, and making individual stories available. But this kind of thing is still far too common:

<blockquote class="twitter-tweet" lang="en">
  <p>
    Give a listen to <a href="https://twitter.com/mizthrush">@mizthrush</a> on CBC discuss Calgary 11th Oil Round action. Starts at 23:30- <a href="http://t.co/ZvXlCD6XKL">http://t.co/ZvXlCD6XKL</a> <a href="https://twitter.com/search?q=%23Indigenous&src=hash">#Indigenous</a> <a href="https://twitter.com/search?q=%23Ecuador&src=hash">#Ecuador</a>
  </p>
  
  <p>
    &mdash; AMAZON WATCH (@AmazonWatch) <a href="https://twitter.com/AmazonWatch/statuses/423160355612020736">January 14, 2014</a>
  </p>
</blockquote>



&#8220;Fast forward to 10:34&#8221; or &#8220;Skip ahead to 23:30&#8221; is a _terrible_ user experience.

The good news is that there are tools and specs built to address this _very_ problem. [Audio deep-linking is possible](http://davatron5000.github.io/TimeJump/). There&#8217;s a whole W3C recommendation for [media fragments](http://www.w3.org/TR/media-frags/). Groups like [Podlove](http://podlove.org/) are actively building tools that address these issues.

Pay attention.

# Vitality, not virality

The subtitle of Alcorn&#8217;s piece comes from this quote:

> “Audio never goes viral,” writes radio and podcast producer Nate DiMeo. “If you posted the most incredible story?—?literally, the most incredible story that has ever been told since people have had the ability to tell stories, it will never, ever get as many hits as a video of a cat with a moustache.”

The thing is, so many people in public radio world _really want_ it to. They want so very badly for audio to be able to (again, pause for cringe) &#8220;go viral.&#8221;

When you stop and think about it, if you swap out the word &#8220;audio&#8221; for something else, the whole question seems a bit silly.

People eat food all the time. Why doesn&#8217;t taste go viral? Almost everyone has a nose. Why don&#8217;t smells go viral? Is it because hip Berlin startup-types have yet to build SmellCloud? I doubt it.

There&#8217;s something more basic going on here, and Alchorn gets at it when he asks:

> is a hit-machine for audio possible? **And is it something anyone even wants?**

Other than radio execs, I&#8217;m not sure anyone does. And I&#8217;m not sure that virality should be a goal for public radio. I&#8217;m not sure it&#8217;s achievable. Past performance suggests it&#8217;s not, at least when we measure success using the metrics of other media.

The last thing public radio needs is a [cargo cult](http://en.wikipedia.org/wiki/Cargo_cult) approach of aping what works for other media, then acting all disappointed when it doesn&#8217;t work out so well for us.

A very savvy CBC executive once advised the Spark team to &#8220;fish where the fishes are.&#8221; I think that applies to CBC Radio more broadly.

Radio excels in certain contexts. For instance, commuting. In Canada, [82% of commuters travel to work by car](http://www.statcan.gc.ca/daily-quotidien/110824/dq110824b-eng.htm). Audio is _great_ in cars, and tech-wise, lots of exciting things are happening in cars: [iOS in the car](http://en.wikipedia.org/wiki/IOS_in_the_Car) and the [Open Automotive Alliance](http://www.openautoalliance.net/#about) to name two. So then, what is public radio&#8217;s car strategy? What is CBC Radio&#8217;s car strategy? Analog transmission?

Part of [CBC&#8217;s mandate](http://www.cbc.radio-canada.ca/en/explore/mandate/ "made available throughout Canada by the most appropriate and efficient means and as resources become available for the purpose.") is to ensure our programming is &#8220;made available throughout Canada by the most appropriate and efficient means and as resources become available for the purpose.&#8221;

I would much rather CBC Radio&#8217;s digital efforts go towards figuring out how to do a better job of what we&#8217;re already good at, rather than trying to get good at making empty-calory web content (listicles, memes, GIFs, etc.) that **simply cannot compete** with the stuff coming out of Upworthy, BuzzFeed, and others.

I don&#8217;t know exactly what digital success for public radio looks like. But I do know getting it right means embracing the best qualities of the medium itself, not shoving radio stories into listicle-sized holes.