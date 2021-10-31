---
title: "Github of Life"
date: 2021-10-31T16:08:35Z
slug: ""
description: ""
keywords: [game, canvas, github]
draft: true
tags: [code]
math: false
toc: false
---
![github of life](/github-of-life-screen.png)

Yesterday I published the [repo](https://github.com/chrisguest75/github-of-life) for [github-of-life](http://github-of-life.herokuapp.com/). It consists of a simple Typescript application and pipeline to deploy it.  The code is a simple implementation of Conway's Game of Life [ref](https://en.m.wikipedia.org/wiki/Conway%27s_Game_of_Life).  Using simple rules to control a cellular grid to create patterns that either life forever or become extinct.  Sometimes you may be left with a set of still or osciallating life forms.   

I wrote it as part preparation for the pairing interview tests that we use at [Trint](https://trint.com).  But I was having so much fun I continued to develop it, the result being the hosted page.  You may notice the github green shades where as the traditional game-of-life usually only deals with on or off cells.  This screen burn effect does not affect the calculations as `1` is still the only live state.  States below this fade out.   

The repo has a pipeline crafted to handle the various stages of the build and deployment process.  It runs jest, linters, container structure tests and scanning - finally deploying to Heroku for basic hosting.  

For convienience I've copied the patterns that are available at [https://www.conwaylife.com/patterns](https://www.conwaylife.com/patterns).  With an extra pattern of my contribution graph.  This is not copied live at the moment.
 
I'll be continuing to work on the `actions` and code to test more aspects of an improved pipeline.  


Links:  
* https://github.com/chrisguest75/github-of-life



