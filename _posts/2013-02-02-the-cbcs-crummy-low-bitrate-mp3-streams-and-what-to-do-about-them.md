---
id: 1606
title: 'The CBC&#8217;s crummy low-bitrate MP3 streams, and what to do about them'
date: 2013-02-02T18:59:21+00:00
author: Dan Misener
layout: post
guid: http://misener.org/?p=1606
permalink: /the-cbcs-crummy-low-bitrate-mp3-streams-and-what-to-do-about-them/
enclosure:
  - |
    http://playerservices.streamtheworld.com/pls/CBC_R1_HFX_H.pls
    0
    application/wordperfect
    
  - |
    http://playerservices.streamtheworld.com/pls/CBC_R1_HFX_L.pls
    0
    application/wordperfect
    
categories:
  - CBC
tags:
  - CBC
  - internet radio
  - mp3
  - Radio
  - streaming
---
About six weeks ago, without any apparent warning, [CBC Radio One&#8217;s audio streams](http://www.cbc.ca/listen/includes/directr1.html) switched from MP3 audio to AAC.

<img class="alignnone size-full wp-image-1607" alt="aac stream details" src="http://misener.org/wp-content/uploads/2013/02/aac-stream-details.png" width="520" height="196" />

This left a number of people unable to listen to streaming audio, namely those with internet radio receivers that don&#8217;t support AAC.

Luckily, a [commenter named Brian let me know](http://misener.org/full-list-of-cbc-music-direct-urls/#comment-17316) that Radio One MP3 streams still exist:

> The trick is to change the “H” to an “L” in the URLs.

Thus,

> http://playerservices.streamtheworld.com/pls/CBC\_R1\_HFX_H.pls

becomes

> http://playerservices.streamtheworld.com/pls/CBC\_R1\_HFX_L.pls

and you get an MP3 stream, compatible with your MP3-only internet radio receiver.

But there&#8217;s a pretty big caveat here. While the MP3 streams still exist, they sound like garbage. Crunchy, low-bitrate garbage. And indeed, they are low-bitrate. They&#8217;re 32kbps MP3s, with a sampling rate of 11025 Hz:

<img class="alignnone size-full wp-image-1608" alt="mp3 stream details" src="http://misener.org/wp-content/uploads/2013/02/mp3-stream-details.png" width="520" height="192" />

_Quick audio lesson:_ the range of human hearing is approximately 20 to 20,000 Hz. There&#8217;s something called the Nyquist theorem that says that to properly reproduce sound, the sampling rate of a digital recording should be twice the highest frequency contained within that sound. If the upper range of human hearing is 20,000 Hz, then you need a sampling rate twice that (this is part of the reason CD audio&#8217;s sampling rate is 44.1kHz).

So, yeah. The CBC Radio One MP3 streams have a sampling rate that&#8217;s 1/4th that of CD audio. They sound crummy. Understandably, this has some listeners frustrated. And for some reason, these frustrated listeners find their way to my blog.

What to do?

This past week, at the CBC Broadcasting Centre, I ran into two people who should have the power and authority to get the MP3 streams back up to a respectable bitrate. I asked them what frustrated listeners should do. The response: [contact CBC Audience Relations](http://www.cbc.ca/contact/) and let them know that you aren&#8217;t happy with the low-bitrate MP3 streams.

Both of the people I talked to were aware of the lowered bitrate, and are building a case for restoring the previous bitrate.

I can&#8217;t pretend to know the myriad reasons why they can&#8217;t just flip a switch somewhere immediately, but apparently, measurable audience feedback is an important part of getting these higher-bitrate MP3 streams back.

So again, if you&#8217;re frustrated by 32kbps MP3 streams, [contact CBC Audience Relations](http://www.cbc.ca/contact/). And tell &#8217;em Dan sent you.