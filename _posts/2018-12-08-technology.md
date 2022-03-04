---
layout: post
title: "City: Technology"
tag: city
date: 2018-12-08
desc: "Looking at a new approach to narrative in city stories."
---

<p style="font-size:10px">Written: 2016-12-01


Working on a fresh story has allowed me to reexamine my thoughts on how to structure a story in this game. As I talked about in [my previous post](http://www.whynotgames.in/blog/city/secondStory), I wanted the narrative in this story to feel more mechanical, and a large part of that was wanting something less linear.

## New Approach To Narrative

I've been playing a lot of *Sunless Sea* of late. Part of this is that it is a game that has something of what I'm looking for from a video game narrative structure. The zailing and the narrative are a little less connected than I would like and the narrative structure is very much derived from Fallen London, which in itself is stat-heavy IF, which is actually really cool, in case my tone didn't convey that. I think that this is an interesting way to make your narrative more interactive. The other part is that I find *Sunless Sea* a lot of fun and their *Zubmariner* expansion gave me another good excuse to get into it again.


One of the most interesting decisions in *Sunless Sea* is plotting out the route you plan on taking from Fallen London. As a result of previous expeditions, there tends to be a number of quests that you can progress at any given point and these quests are all tied to specific islands. Figuring out an optimal route that goes through a number of these islands and lets you pick up some bonus cash on the way is quite engaging. You are encouraged to do this by the game as by plotting out a route, you can pick up the things you expect to need for various stories in Fallen London before setting out.


What I like about this system that I would like to use:
- The looping feel of the narrative.
- How multiple narratives intertwine because it is sub-optimal to just focus on one at a time.
- Diversions from the major storyline that the player is currently following.
  



I am worried about needing a wiki to play the game as a result of this though.


Components that I need to recreate:
- States with story implications associated with them that are closer or farther from other states.
- With this, I need value for the player in going to nearby states that do not have immediate story implications.
- A home state.
- The ability to carry over some kind of state from island to island.
  



I'm going to experiment with morphing traits as a way to get here. This also lets me put a lot more traits into a game that breaks down a little with more than 5 defined traits at any given moment. How I plan for this to work is for the player to be able to transform some traits into other traits in a cyclical manner with some nodes having multiple branches. Some of these transformations will require other states to be active and as of now, I'm timing some of the states as well.


This probably seems a little arcane right now, but once I've finished experimenting with it, I'll attach an image, which should make it much clearer.


One of the things that really helps with this is having goal buttons instead of having to have all of the possible goals on the screen. This additionally lets me obsolete the old linked goal technology, which was anyway an opaque mechanic.

## Conclusion

This is probably not the most satisfying of articles as at best it illustrates the problem without actually proving the solution. It is a lot of things that I'm very excited about though, and if my experiments pay off, my next article will be able to demonstrate the solution clearly.


