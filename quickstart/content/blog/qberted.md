---
title: "Qberted"
date: 2021-10-31T16:22:38Z
slug: ""
description: "Qberted perpetual grid"
keywords: []
draft: false
tags: [code]
math: false
toc: true
---

![qberted](/qberted.png)

Retro gamers must all know about Q\*Bert an early isometric grid game.  I started out trying to create the same grid effect as a background, but with a perpetual falling of the stacks. It turns out there were some little tricks I had to consider along the way. 

[QBerted](https://qberted.herokuapp.com/)  

With an effect like this we want to reduce the amount of overdraw. If the stacks were full size we'd have to draw each stack from the top to the bottom of the screen. When in fact most of it is obscured by the stack in front. We also want to control the amount that a stack can fall so as not clear too much of one stack or another.  

Luckily SVG uses order in the DOM as the draw order and therefore no `z` coordinate is required.  We just use `x` and `y` to control the positions of the top of the stack.  The rows alternate with an offset to create the isometric effect - this is important when replacing rows at the top after other have clipped off the bottom of the screen.  

The stacks are chosen at random to move and then will only move if the columns above and below will not differ in distance by three cube heights.  

It's a fun little perpetual effect that also rescales to be fullscreen if required.  
