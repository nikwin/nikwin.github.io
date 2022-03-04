---
layout: post
title: "City: Consolidation"
tag: city
date: 2018-11-9
desc: Work done on consolidating my game.
---

<p style="font-size:10px">Written: 2016-02-10


My work of late has been focused on consolidating the game. A lot of technical, visual and design debt has been cleared as a result. This has, of course, made it much easier to do more work on the game. This has also made the game itself much more fun to play, which is a side effect that I did not really expect this soon. Enough has been fleshed out to lead to the trade-offs that make for interesting decisions.

## Screenshot

First of all, the game now looks clear enough for me to put up a screenshot. It still looks far from acceptable let alone finished. The art is just enough for me to be able to test out mechanics and no more. It's going to look terrible for quite a while more, but nevertheless, here is the first screenshot of the game.

<img src="/blogImages/SS_2016-02-10_01.png" />
## The Will System

Will is the primary currency of the game. The player needs to spend will to do things like build new towers and start new tasks. Earlier, will would be generated in chunks every fifth of the day and so the game had bursts of activity followed by long periods of waiting. Now, will regenerates when the focus level is kept low where the focus level is determined by the number of towers the player has active at a given time.


This both makes the focus system generate interesting decisions and lets me remove the system for the parts of the day. These were far and away the two weakest systems in my game and being able to strengthen one and remove the other did a lot to make the game more playable.

## Tower Abilities

From [my system analysis](/blog/city/systemAnalysis), I felt that the game needed more scope for player expression. Building towers is the primary action that players can take and so seemed like a good starting point.


There are now multiple towers that can complete certain goals. This lets the player choose which one they identify the most with, but these towers need to be different in more than just name. So, I added support for what are essentially different damage patterns. Additionally, the mix of currencies generated varies from tower to tower.

## Associations

Another mechanic that I wanted to try is generating associations with the actions that players commonly take. I thought that this would add some weight to player decisions and so may add to the feeling of self-expression. I now think that was incorrect and none of these features really do anything for player expression. I think that the core of adding self-expression is not just being able to make impactful decisions, but to let the decisions be guided by player whims. Nevertheless, some pretty cool features came out of the experiment.
- <b>Unused entities lose health</b> - I like having the map react to the player and this helps represent the person changing with time. This also naturally removes things that the player isn't interested in anymore, which saves the player manually removing them when they need the space.
- <b>Creep associations</b> - Whenever a source generates a creep, it has a chance of associating that ability with that creep. If this happens, whenever that activity is used it will generate that creep. So, when doing your chores gets associated with disgust, doing any chore will result in disgust from then on. This association is an item that can be killed like other items by completing the actions associated with it. So, you can then end this association by writing about it in your diary for instance. I really like the interaction of being able to remove these associations a lot though.
- <b>Damage boosts</b> - Similarly, I had towers that continuously damage a kind of creep gain bonus damage against that kind of creep. This feature did nothing and so I killed it. It's conceivable that by inverting creep associations I could get it to be satisfactory, but for now it is simply dead.
- <b>Tower Source Leveling</b> - This needs to be worked on a little bit more before I can judge it. Right now, it caps the number of towers of a single type that you can build, which is a change that I really like. Pushing players to build a wider range of buildings leads to more interesting play and this does that, if in a very direct way. Also, I have high hopes of leveling up your abilities through using them as a general mechanic.


## Minor points

<b>Random Events</b> - These are a mechanic that I've always liked and now that the game is playable, this is really starting to work out. It forces people to recalculate what they are doing at unexpected points and these calculations are much of the fun of this game.


<b>Emotion Peaking</b> - Having any emotion peak now has dramatic effects. I need the player to keep track of their emotional state as the tower defense parts of the game rely on that and so emotions need to have effects. Also, this maps well from real life.


<b>Non-damaging towers</b> - I've struggled for quite a while with trying to figure out which emotions I deal with by working and I no longer think that metaphor makes sense. Working gives me something to focus on until the emotions die down, which is fairly interesting to represent mechanically. I already monitor the focus system for will generation, having it suppress creeps is trivial and creeps already lose health with time. I feel this metaphor to be a lot closer to reality than trying to shoehorn emotional effects into every tower. However, activities like taking walks still directly impact emotions.

## Conclusions

I'm going to spend some more time working on making the map responsive and giving the player more scope for self-expression. These seem like the points where the game is furthest from being completed. Having the game prove fun at this stage is very unexpected and frees me up enough that I can work on this axis instead.

