---
title: "Spaceballs Dancer"
date: 2021-10-31T20:11:05Z
slug: ""
description: "Based on an old Spaceballs demo"
keywords: [demo, code]
draft: false
tags: [demo, code]
math: false
toc: false
---

![dancer](/dancer.png)

Those who remember the old Amiga demoscene might recall "State of the Art" by the Spaceballs.  At the time this was ground breaking with a vectorised dancer moving around fullscreen with clipping.  It was all but an MTV video with dance music and fast strobing visuals.  

As a member of some retro groups that regularly post youtube videos of them.  After seeing it again I decided to have a go at recreating it.  

I found a video online of a dancer going through a routine that I downloaded using youtube-dl and then imported into Adobe Premier to find a small loop.  
Once exported I used ffmpeg to output each frame to jpgs.  At 30fps this created around 60 images that I loaded into gimp as individual layers.  Using the magic wand and lots of patience I removed the background from each one.  It took a while and I'm still searching for a free piece of software that could help here.  Or next time I'll find a green screen dancer perhaps.  

Once all the frames had been saved individually back out from the layers, they were processed through a cli tool to create them as SVG.  These points were then extracted using a quick script and loaded into a json document.  

Running out of time to put a music player on it - I'll revisit it at some point.  


