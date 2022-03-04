---
layout: post
title: City: Further Analysis
tag: city
date: 2018-11-15
desc: A deep analysis of the mechanics of City.
---

<p style="font-size:10px">Written: 2016-04-03

<img src="/blogImages/SS_2016-04-04_01.png" />

The beginning of this month marked the point where I start focusing on getting a playable version of the game out. The first step that I wanted to tackle was stock-taking. The core of the game remains as detailed [here](/blog/city/core) and you can read the previous system analysis [here](/blog/city/systemAnalysis).


This follows a slightly different structure than my earlier analysis. Here, I list both aesthetics and the game dynamics that can result in those aesthetics. I then examine the pieces of the game to see what they contribute to and so see which are not pulling their weight.

## Aesthetics

The desired aesthetics are the same as in the previous analysis. They are:
- Familiarity in novelty / self-discovery
- Challenge
- Narrative
- Expression


## Dynamics

These are interactions between game pieces that result in the player experiencing the aesthetics above. This is obviously non-exhaustive.
- <b>Choosing which action to take</b> - This is essentially just the manifestation of the aesthetics of challenge and expression. You don't have challenge or space for expression without the ability to make real decisions.
- <b>Building up emotional state or will</b>
- <b>Developing personality</b>
- <b>Needing to adjust your day due to random events.</b> - This is critical for a lot of the game. It is an integral part of generating narrative and challenge and is also key to the aesthetic of novel representation as well. This dynamic ties together a large amount of the game and benefits deeply from doing so. Examples for this include being unable to hit your work target for a day because you wake up depressed and avoiding talking to people because an incident on your commute has made you angry.
- <b>Needing to deal with emotions</b> - Much of the previous point applies here as well. The emotions are the antagonist of the tower defense parts of the game, and so it is necessary that they be impactful as otherwise players will just ignore that side of the game. Additionally, a representation of the mind that ignores the importance of emotional state on decision making would be deeply flawed.



Additionally, I would like better support for the dynamics of viruses, where activities are associated so deeply with an emotion that the player can no longer use them and for the dynamics governing the generation of traits.

## Mechanics

This is not a full listing of the entities and systems in place in this game as many of them are there for bookkeeping behind the scenes and are not something that the player needs to worry about. While I agree that the game might be better if the entity for the buttons, for example, were so deeply integrated into the game that they merited analysis of this kind, that seems non-essential at this stage and additionally would come with a complexity cost.


I've listed all of the pieces that players will have to care about and the dynamics and aesthetics that they contribute to.

<table border="1px">
<tr><th></th><th>novel</th><th>narrative</th><th>challenge</th><th>self-expression</th><th>choosing action</th><th>building up</th><th>development</th><th>adjust day</th><th>deal with emotions</th></tr>
<tr><td>creep</td><td>X</td><td>X</td><td>X</td><td></td><td>X</td><td>X</td><td></td><td>X</td><td>X</td></tr>
<tr><td>boosts</td><td></td><td></td><td></td><td>X</td><td></td><td></td><td>X</td><td></td><td></td></tr>
<tr><td>wish</td><td></td><td>X</td><td>X</td><td></td><td>X</td><td></td><td></td><td>X</td><td>X</td></tr>
<tr><td>emotionCurrencyTicker</td><td>X</td><td></td><td>X</td><td></td><td>X</td><td>X</td><td></td><td></td><td>X</td></tr>
<tr><td>emotionSentinel</td><td>X</td><td>X</td><td>X</td><td></td><td>X</td><td>X</td><td></td><td>X</td><td>X</td></tr>
<tr><td>item</td><td>X</td><td>X</td><td>X</td><td>X</td><td>X</td><td>X</td><td></td><td>X</td><td>X</td></tr>
<tr><td>memory</td><td>X</td><td>X</td><td>X</td><td></td><td></td><td></td><td>X</td><td>X</td><td></td></tr>
<tr><td>path</td><td></td><td></td><td>X</td><td></td><td>X</td><td></td><td>X</td><td></td><td>X</td></tr>
<tr><td>person</td><td>X</td><td>X</td><td>X</td><td></td><td>X</td><td></td><td>X</td><td>X</td><td></td></tr>
<tr><td>producer</td><td>X</td><td>X</td><td>X</td><td>X</td><td>X</td><td>X</td><td>X</td><td>X</td><td>X</td></tr>
<tr><td>trait</td><td>X</td><td>X</td><td>X</td><td></td><td>X</td><td></td><td>X</td><td>X</td><td></td></tr>
<tr><td>spell</td><td>X</td><td>X</td><td>X</td><td></td><td>X</td><td>X</td><td></td><td>X</td><td>X</td></tr>
<tr><td>Damage System</td><td>X</td><td>X</td><td>X</td><td>X</td><td>X</td><td></td><td></td><td>X</td><td>X</td></tr>
<tr><td>Tick Emotion System</td><td>X</td><td>X</td><td>X</td><td>X</td><td>X</td><td>X</td><td>X</td><td>X</td><td>X</td></tr>
<tr><td>Emotion Source System</td><td>X</td><td>X</td><td>X</td><td></td><td>X</td><td></td><td></td><td>X</td><td>X</td></tr>
<tr><td>Source System</td><td>X</td><td>X</td><td>X</td><td></td><td>X</td><td></td><td></td><td>X</td><td></td></tr>
<tr><td>Map Spawn System</td><td>X</td><td>X</td><td></td><td></td><td></td><td></td><td>X</td><td></td><td></td></tr>
<tr><td>Wish Make System</td><td></td><td>X</td><td>X</td><td>X</td><td>X</td><td></td><td></td><td>X</td><td></td></tr>
<tr><td>Make Memory System</td><td>X</td><td>X</td><td>X</td><td>X</td><td></td><td></td><td>X</td><td>X</td><td>X</td></tr>
<tr><td>Execute System</td><td>X</td><td>X</td><td>X</td><td></td><td>X</td><td></td><td></td><td>X</td><td>X</td></tr>
<tr><td>Tick System</td><td></td><td>X</td><td>X</td><td>X</td><td>X</td><td></td><td></td><td>X</td><td>X</td></tr>
<tr><td>Focus System</td><td></td><td>X</td><td>X</td><td>X</td><td>X</td><td>X</td><td></td><td>X</td><td>X</td></tr>
<tr><td>Emotion State System</td><td>X</td><td>X</td><td>X</td><td></td><td>X</td><td>X</td><td></td><td>X</td><td>X</td></tr>
</table>

Note that the columns represeting dynamics are only meaningful in that those dynamics result in aesthetics. The clear weakest piece is the boost. It just does not do enough of anything and the effect that it has on self-expression is not enough for me to leave it alone. There are issues that the game needs to solve that I can see it helping with, but it is something that I need to keep an eye on and possibly cut.


Additionally, my analysis showed me the following pieces:
- Tower Emotion Associations - These are towers generating emotions when active. This can be folded into the memories.
- There are three different systems that all make other entities. From a code perspective, these should be merged into one.
- Modifying currency production due to emotion, making entities that change the difficulty of various goals and making entities based off active emotions and sources are all interesting things that need better integration.
## Conclusion

There are quite a few things that could still be worked on, but the table of mechanics is actually very reassuring. With just one exception, the pieces all seem to be in a reasonable place. There's room for improvement, but there are worse places that I could be at this stage.

