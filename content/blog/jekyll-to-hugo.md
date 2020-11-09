---
layout: post
title: Goodbye Jekyll, Hello Hugo
aliases: 
date: 2020-11-09
tags:
- meta
---

I don't know why I picked election week to finally bite the bullet and redesign my site in [Hugo](https://gohugo.io/) after using [Jekyll](https://jekyllrb.com/) for over four years, but I did. Do things look different around here? Maybe a little snappier? That's the power of New and Fresh Code™. 

<!--more-->

For context: Jekyll and Hugo are what are called "static site generators," computer programs one can use to compile more or less totally self-contained HTML sites from things that are easier to write than HTML, like Markdown. Theoretically, they make developing a website so much easier than heavy database-powered programs like Wordpress. In practice, they're just as needlessly complicated as anything in web development these days. There are a million different static site generators and I low key love and hate them all in equal measure. 

Jekyll was the big one for many years: it was the first and the most widely supported. There was—and still is—a substantial community around it, which was nice for the kind of programmer that I am, which is a poor one. GitHub could host a Jekyll-powered site natively through its Pages product, and I used that more or less happily for many years. 

However, Jekyll's got a few downsides that became glaring in the past twelve months or so. For starters, it gets really slow to work with really fast. I have about seventy blog posts and some moderately complex templates that render things like my [CV](/cv) from a single data file.[^1] Once youthful and spry, Jekyll would routinely take three or four seconds to render my site when developing it locally. I know that doesn't sound like much, but trust me it's just enough to be annoying—plus some tests I ran indicated it was only going to get exponentially slower the more pages and posts I added over time. 

[^1]: Why? Because I use that same data file to produce a .pdf version using LaTeX. Yes, I am completely insane—but you knew that already. 

The second issue is that GitHub (a company I am ambivalent about in the best of times!) has increasingly made clear that they're not really going to support the Pages product that much going forward, and aren't really invested in Jekyll being a part of it. Jekyll's on version 4-point-something, but GitHub still only supports 3-point-something. I've started getting weird errors from all its Ruby dependencies. And if there's something I don't have time for when I'm trying to finish a dissertation and get a job in the middle of a pandemic, it's weird errors. 

So! I decided to finally pull the plug and shift to the Hot New Thing, Hugo, which is a static site generator built in Go, which I think is Google's programming language? Honestly I do not care one whit about all the techie ins and outs, other than from a bunch of searching I got the sense that Hugo was the next-best-supported option after Jekyll.

I will say however that Hugo has two clear advantages over Jekyll: 1) it is extremely fast; and 2) it is a binary file, so there aren't dependencies to muck around with. Porting my site over was a pain in the neck (I won't go into too much detail about how I did it, because what I learned is that it's really a case-by-case basis for how to port a Jekyll site to Hugo so my advice will not really help you much, sorry! Plus there are like, seven million posts out there running through the same thing) but it's done now. Plus I got to use a spiffy new theme with some minor variations and adjustments to keep long-time readers on their toes. It runs on a service called [Netlify](https://www.netlify.com/), which I think I get about thirty percent of because it's wrapped in very Amazon AWS-y enterprise language. I don't think I'm going to get charged at any point? But we'll see!

(And in doing this port, I have in fact broken a solemn vow I made to myself not to mess with my website until I had finished my diss, because the old version worked perfectly well and it was really just advanced procrastination. To which I say: oh well, who cares, I just spent the past week glued to my phone to see who was gonna be president so I deserve the procrastination.)