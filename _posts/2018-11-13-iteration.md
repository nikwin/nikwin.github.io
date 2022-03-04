---
layout: post
title: 'City: Iteration'
tag: city
date: 2018-11-13
desc: Growth and pruning of existing city features.
---

<p style="font-size:10px">Written: 2016-03-17


I've done a lot of work to try to make the various pieces of the game make more sense. There's been some amount of pruning and some amount of growth as a result. A lot of this work has been quite successful, but there is one critical feature, the people, that still needs a major change.

## Screenshot
<img src="/blogImages/SS_2016-03-17_01.png" />
## Insights

I put in insights last sprint ([here](/blog/city/construction)), but they were more confusing and fiddly than fun. Now, instead of having them be a piece for the player to manage, they are just added automatically to the relevant towers. This means that they no longer function as a piece for self-expression, but they do work as a reward, as a growth indicator and as a reflection of how the player has played thus far. So, while they do not function as a self-expression piece, but they do reinforce the self-expression found in other pieces.

## Actions To Hurt/Heal Traits and Sources

At first, this feature was very direct. You were able to essentially write in your diary about how much you love sport to reinforce the idea that you love sport. Procedurally generating this, such that you could use it to heal or hurt any entity didn't fit mechanically or narratively. It gave too much control to the player for either half to be successful.


Instead, success and failure for a number of actions and random events can result in a health difference for other entities. This adds expressiveness to the actions and allows the player more control over the health of their traits. It requires more handwritten parameters though and players are more likely to find themselves in situations which feel inescapable. On balance though, this seems to have been a positive tweak.

## People

I did a lot of work on people (last expanded [here](/blog/city/construction)) and they have more flesh on them now, but I feel that the feature is still in need of a key transformation.


Nevertheless, social actions now have social effects. Your relationship with a person deteriorates over time, and you can use social actions to help rebuild the relationship or to damage it further. Additionally, people now have traits that help determine their behavior and spending time with them lets the player learn what they are.


Additionally, other people now request that you do stuff with them. This is once again based off their traits and relationship health and brushing them off will impact the latter.

## Removing Tower Sources

This was far and away my greatest success from this set of features. I've merged the tower source system (first described [here](/blog/city/towerLife)) and the personality trait system (described [here](/blog/city/pieces)) so that personality traits unlock actions and generate the combined emotional output of all of them.


This plays extremely well. It removes a piece that was unnecessary for communication and made the map more compact and more interesting. Mixing together the output of various towers makes the decision of which towers to place along the line substantially more interesting.


Additionally, it's made some older features play better. Now, limiting the number of towers by the source level applies across all the towers of a trait instead of just all of the towers of a type and so makes for interesting trade-offs. I also tweaked the experience system so that things level up more with use and made leveling up result in the trait growing an extension in a new hex. So, traits now end up sprawling out across the map as you develop them further and further.

## Memories

Now, memories (first implemented [here](/blog/city/construction)) show up on the map instead of just the UI. They pop up at the same times, but actually having them take up space in the surrogate's mind naturally emphasizes their existence. They now also generate flashbacks which create a burst of one of the emotions remembered at one of the traits associated with that memory.

## Time Bombs

Time bombs are essentially repeating events which penalize you for failure. For instance, not getting enough exercise damages the player's will and makes them frustrated. This both gives the players some plates to spin and lets me add more plates as the player develops, forcing them to adapt. I don't want the player to feel superhuman and adding maintenance costs to development lets the game focus on transformation instead of plain progression.

## Conclusion

This did a lot to make the mind feel less predictable and helped make the game metaphors feel like less of a stretch. There's still a bit more work to do on this front and a lot of breadth that needs to be added. However, we're still closing in quickly on moving to the next stage, which is being able to focus on making all of these pieces presentable.

