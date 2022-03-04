---
layout: post
title: City: First Playable
tag: city
date: 2018-10-30
desc: Description of the first playable version of my game.
---

<p style="font-size:10px">Written: 2015-12-8


I've just finished the first playable version of this game. Some things have gone pretty well, some are not where I want them to be. Writing for this game is going substantially better than I expected and I'll go into more detail about that shortly. The goal of the work that I've done up to this point was to see if it looked like the experience I want to create is feasible. That goal seems to have been achieved, I believe that there are the bones here of the game I want to see. Besides that, I've also seen the following:

## Writing Scenarios

This is really where things are going better than I expected. I can now represent emotions, actions and mental state to a degree that is functional. It is naturally still quite far from what I would like it to be, but the core seems solid and building out from here seems relatively easy. I can now represent scenarios from a person's life fairly easily. I could make this my new diary and quite possibly will.


About half of my work for this version has been on tools. When starting work for this goal, I found creating content to be close to impossible. Sharp tools make work like this substantially easier and substantially better. Simply removing boilerplate helps you keep track of all of the data you need which makes a very meaningful difference in the work you create.


While these scenarios function as snapshots, the simulation aspects of the game are almost non-existent and so the experience falls apart very quickly. Essentially, you can get everything that the scenario has to say within a few minutes of starting the scenario and that information is really just a glorified list of points detailing emotions and activities of the time.

## Gameplay

The gameplay is currently nothing short of terrible. This is not really a surprise. Right now, I have a very minimal tower defense game and I think that the gameplay in those games tends to be terrible as well. The pure mechanic of placing towers by a fixed path to destroy the maximum number of creeps is just a weakly disguised spreadsheet. Despite this, most tower defense games are fun as they layer elements over their core like:
- Theming - Plants vs. Zombies is an excellent example of this.
- Action components - Space Run, Orcs Must Die and Sanctum all do this. 
- Progression Systems - Being able to build more and better towers is a meaningful form of progression as shown by Clash of Clans.
- More varied content - Varied towers and varied creeps can push a game like this further, especially when some of them work in a fundamentally different way, like the sunflowers in PvZ.



It's not surprising that the game is not that fun at this stage, the systems do not support any interesting decisions and the theme is not integrated. I believe that improving the simulation will also make the decision making of which tower to place deeper and easier to parse for players. Nevertheless, this is something to keep an eye on.

## What I'm Doing Now

The shallowness of the simulation seems to be the biggest issue both with the expressiveness and the fun of the game. I'm going to start by making the towers more dynamic. I'm going to try the following pieces:
- Linking like towers together and making them output creeps of their own in certain cases. This should make each person's map grow out organincally as they build towers to help deal with the output of other towers.
- Add controls to the towers. I don't want the game to become action oriented, but I like giving players more control over parts of their lives. I want this to feel more like being able to shift parts of a factory line than an element of micro-management.
- Giving towers a chance of creating events to help flesh them out. For example, the tower representing working could generate events like projects going well.
- Global mood affecting towers. Firstly, this adds verisimilitude to the simulation. I can't work well when I'm furious about something and this is a way to represent that interaction. Additionally, it adds secondary effects to player actions, which makes the decision of which tower to build a little less trivial. It does not necessarily remove the spreadsheet aspect of the genre though. I'm going to get the simulation aspects of the game to be a little more functional before I audit the decision making aspects though.



