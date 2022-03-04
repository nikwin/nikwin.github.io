---
layout: post
title: "City: Towers, Focus and Emotion"
tag: city
date: 2018-12-10
desc: Looking to fix the issues with a few systems of city.
---

<p style="font-size:10px">Written: 2016-12-24


The nexus of the tower, focus and emotion systems have always been good in theory but have never played out well. I don't really have the time right now to monkey around with systems, but I'm unhappy enough with the way they run that I'm going to do it anyway. Before I jump in though, I'm going to take a moment to detail out what these systems do well and why they are lacking.

## Aesthetics

As a reminder, the driving aesthetics of the game are:
- Familiarity in novelty / self-discovery
- Challenge
- Narrative
- Expression



You can read the explanation of this in my first system analysis article [here](/blog/city/systemAnalysis)

## Damage Towers

This feature decomposes as follows:
- Emotions take the form of tower defense creeps and come down lanes trying to reach the id of the player, which causes the player to lose control of their mind.
- Certain towers, such as callousness, damage these emotions as they pass by.
- These towers require resources, such as will, which are fed to it in the same manner as the other towers.



I feel that this feature does really well on the first and most important aesthetic. The idea of listening to music to calm yourself, for instance, is very flavorful and clear to the player. Theoretically, this is also great for challenge, but in practice it doesn't do much there. I'm okay with where it is on narrative and expression although it could do better on the latter.


The biggest issue with this is that the micro of turning them on and off is just not fun. It's a chore with nasty consequences if you forget to turn them on. There's no interesting decision to be made here.


When you compare the tower building of this game to that of traditional tower defenses, it is clear that it just is not good enough. The positioning is there, but that is really all that it manages. Part of this is just in the numbers. There are too few damage towers and too few creeps to really feel like a tower defense or give players the scope to really engage with it.


Additionally, the information of what emotions are coming is just not communicated well, which makes it hard to make decisions.

## Emotions

These are pretty much the other half of the system described previously. They are the creeps that the towers kill. Additionally, they create traits that can have towers and goals built on them as well.


Again, they do well in theory across the four axes. Losing control of yourself because of how sad you are is great storytelling. Using frustration at a personal insult to fuel yourself to do more is basically every day for me.


However, I feel like they still do not do enough. As a player, I don't have to think enough about them. Their answers are generic and their currencies are inessential. Additionally, they are interchangeable. Having something make you angry doesn't feel enough like it is making you angry right now, and it doesn't feel very different from when you are happy.

## Focus System

This feature decomposes like this:
- Every goal takes a train of thought to complete. This train goes through all of the towers necessary to produce the currency that the goal needs.
- The player can only have so many trains of thought active at any given point of time.
- The more trains that a player has active at once, the less efficient their production is.



Again, I really like the flavor of this feature. In particular, I love how cleanly it represents keeping yourself too busy to be emotional. The mechanic is fairly elegant as well. It's easy to understand, plays well with the other mechanics and requires different answers at different times. Also, I love the way you can stockpile a resource when things are quiet and then burn through it when things get busy.


The biggest problem with this feature is how disconnected it feels from the player's decisions. While this is something that a player can grasp as an abstract concept, it is hard to develop any kind of intuition as to how exactly it really plays out and so it is hard to work it cleanly into one's decision making process.

## Potential Solutions
## Making The Game Turn Based

Changing the cadence of the game would do a lot to help with the clarity issues that seem to be a large part of the problem. However, this is a drastic change and so I would need to believe the potential upside to be high enough to offset the risk. At this point, that does not seem to be the case.

## Remove The Currency Requirement For Towers

By removing the currency requirement for towers, they can always be on which removes the highly irritating micro from them.


On the other hand though, we lose the narrative of requiring currencies to perform these actions. This is a consistent part of the game and having damage towers require it makes the systems interact better with each other and it adds an additional cost to being emotional. Not having the will to perform additional actions because you're too busy keeping a handle on your emotions is powerful storytelling to lose.

## Have A Global Tick To Clarify The Focus Issues

I want to try just making the focus clearer before meddling too much with it. It's an elegant system and I have a terrible weakness for those. I'm going to try using a global, visible tick and tie all of the processing that would normally use the focus to that instead.

## Increase The Flow of Emotions

By constantly having emotions flow down the paths we can eliminate the need to turn towers on and off constantly and so reduce the micro. The issue is that this also reduces the decision making of the towers. It works out to the same as removing the currency, but from the other side. That is, it once again takes away the storytelling of trading off dealing with emotions, but in this case it does so by forcing the player to always have the towers on.

## Create More Towers of The Emotion Source Immediately

Emotion traits can provide the player with more efficient ways to get things that they want, but often requires more effort from the player as the player may have a way to generate those currencies already. By having some of these towers pop up immediately, that encourages players to use these traits more.


I can also make the way that they die with time use the technology of timed world goals that I developed for songs.

## More Emotion Explosions

I like the idea of losing control resulting in major transformations of things on the map. For instance, trying to convince a person should blow up into shouting at that person when you become angry. This helps emphasize their differences and makes them more tactical.


The issue is that losing control is something that players intrinsically do not want to do. Much of the game is about handling emotions and asking players not to do that will go against their instincts unpleasantly. Also, making sure that only the emotion you want will get through is difficult.


Players just do not have the tools that they need for me to make this a fundamental part of the game. It is still interesting to see though, so it won't completely disappear.

## Powering Up Towers

Essentially have the towers have a default state and then be able to charge them for more efficacy. In the same way, I can change the emotion generation to have an immediate feeler and then push a real wave through shortly afterwards. This will help deal with the communication issues while still keeping the feature interactive.

## Building Up Towers

One of the big issues is just that there is not enough space to have enough towers to make this feel like a tower defense. The simple solution is to essentially put multiple towers in the same space by letting players build up a single tower.

## Proposed Solution

I'm going to try the global tick, the immediate emotion towers and powering and building up towers and see how that works out.

