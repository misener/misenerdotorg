---
id: 885
title: Computers get smarter, CAPTCHAs get harder
date: 2011-03-01T09:40:38+00:00
author: Dan Misener
layout: post
guid: http://misener.org/?p=885
permalink: /computers-get-smarter-captchas-get-harder/
onswipe_thumb:
  - 'http://misener.org/wp-content/plugins/onswipe/thumb/thumb.php?src=http://misener.org/wp-content/uploads/2011/03/Captcha.jpg&amp;w=600&amp;h=800&amp;zc=1&amp;q=75&amp;f=0'
categories:
  - CBC Radio technology column
tags:
  - CAPTCHA
  - Luis von Ahn
---
This week&#8217;s CBC tech column ([CBC.ca version](http://www.cbc.ca/news/technology/story/2011/02/28/f-vp-misener-captcha.html)) is all about CAPTCHAs, and how some of them are getting harder. CUE OMINOUS VOICE. The robots are getting smarter.

[Audio to follow]

===

[<img class="alignnone size-full wp-image-889" title="Captcha (1)" src="http://misener.org/wp-content/uploads/2011/03/Captcha-1.jpg" alt="" width="200" height="70" />](http://misener.org/wp-content/uploads/2011/03/Captcha-1.jpg)[<img class="alignnone size-full wp-image-892" title="Captcha" src="http://misener.org/wp-content/uploads/2011/03/Captcha.jpg" alt="" width="200" height="70" />](http://misener.org/wp-content/uploads/2011/03/Captcha.jpg)

Tell me if this sounds familiar: you&#8217;re online, ready to buy some concert tickets or to sign up for a new email account. But before you&#8217;re allowed to proceed, you have to prove you&#8217;re a human being by deciphering a mess of distorted, squiggly letters and numbers, then typing them into a text box. This is what&#8217;s called a CAPTCHA, or completely automated public Turing test to tell computers and humans apart.

For a while now, I&#8217;ve had a sneaking suspicion that CAPTCHAs are getting harder. Increasingly, I&#8217;m left wondering, Is that an uppercase &#8220;x&#8221; or a lowercase &#8220;x&#8221;? An &#8220;o&#8221; or a zero? A &#8220;q&#8221; or an &#8220;o&#8221; with a squiggle through it? Sometimes, even though I&#8217;m 100 per cent sure I&#8217;ve typed exactly the right thing, the computer disagrees with me.

For months, I thought I was alone in this frustration. I worried that my increasing inability to pass these tests suggested that I&#8217;m not entirely human.

Then last week, I opened an email message from a colleague that read: &#8220;You know those distorted letters we have to type to pass security tests online? I notice they&#8217;re getting more and more distorted.&#8221;

According to [Luis von Ahn](http://www.cs.cmu.edu/~biglou/), one of the computer scientists who coined the term &#8220;CAPTCHA,&#8221; the tests are getting harder.

&#8220;The thing about CAPTCHAs is that many people do their own implementations,&#8221; he told me. &#8220;Over time, some of these implementations have gotten a lot harder, because the really easy ones &#8211; essentially, the undistorted ones &#8211; can be broken by bots.&#8221;

Traditionally, identifying squiggly, distorted letters has been difficult for computers but comparatively easy for humans. But computers are getting better and better at it, and easy CAPTCHAs aren&#8217;t as effective as they once were.

Still, von Ahn says his own implementation of CAPTCHAs, called [reCAPTCHA](http://www.google.com/recaptcha) , isn&#8217;t getting any harder.

&#8220;It&#8217;s still the case, as it was three or four years ago, that a person who submits a solution [to reCAPTCHA] is going to be correct 96 per cent of the time,&#8221; von Ahn said. &#8220;That number remains the same.&#8221;

ReCAPTCHA, which was acquired by Google in 2009, generates more than 100 million CAPTCHA images a day for various websites for free. The CAPTCHA images it provides are also used to help decipher words that can&#8217;t be identified during the process of digitizating printed material.

Computers are getting better at solving CAPTCHAs because devising automated ways of bipassing the test is potentially lucrative. Imagine that you&#8217;re an email spammer. Wouldn&#8217;t it be great if you could automatically sign up for hundreds or thousands of bogus email accounts? Or, imagine you&#8217;re a ticket scalper. Wouldn&#8217;t it be terrific if you could write a computer program to automatically buy all the tickets for a concert? CAPTCHAs can help keep spammers and scalpers at bay.

Because there&#8217;s a lot of money to be made, software developers are actively writing code they say can crack CAPTCHAs that, von Ahn says, sells for $10,000. Von Ahn said he has even seen ticket scalpers advertise software they say can break reCAPTCHA for as high as $50,000.

According to von Ahn, it&#8217;s simply a matter of time before software will rival humans at solving CAPTCHAs, but it could take decades.

In the meantime, as easier, ineffective systems are phased out, people will continue to be frustrated by some CAPTCHAs. And as frustrating as CAPTCHAs are for the average user, they can be even more frustrating for people who are visually impaired or use screen-reader software. Some CAPTCHA implementations include an audio alternative, but accessibility will continue to be an issue.

Regardless of how they are implemented, CAPTCHAs are all built around the idea of creating a task that&#8217;s hard for computers and easy for humans. As computers get better and better at reading squiggly letters, we may be asked to prove our humanity by performing other types of tasks.

For instance, computers are still very bad at determining the contents of a photograph. It&#8217;s difficult for software to tell the difference between a photo of a cat and a photo of a dog. Microsoft Research built a CAPTCHA system called [ASIRRA](http://research.microsoft.com/en-us/um/redmond/projects/asirra/) (Animal Species Image Recognition for Restricting Access) based on this idea. Companies like [Solve Media](http://www.solvemedia.com/) and [NuCaptcha](http://www.nucaptcha.com/) have put their own twists on CAPTCHAs that require users to enter words from a text or video advertisement.

If von Ahn is right and computers will eventually be able to reliably solve text-based CAPTCHAs, that&#8217;s not necessarily a bad thing. Though CAPTCHA-busting technology could be used by spammers or ticket scalpers, it could also help decipher hard-to-read parts of digitized books or identify skewed and distorted text in photographs.

So, the next time you&#8217;re confounded by a mess of squiggly, distorted letters, don&#8217;t be too hard on yourself. Maybe it&#8217;s the CAPTCHA&#8217;s fault.

As von Ahn told me, &#8220;Sometimes, they&#8217;re really bad. Sometimes, they are so hard to read that I can&#8217;t read them myself.&#8221;

Comforting words from one of the people responsible for all those squiggly letters.