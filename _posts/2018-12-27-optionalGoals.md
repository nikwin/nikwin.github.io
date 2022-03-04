---
layout: post
title: The Anti-Pattern of Optional Goals in Tasklists
tag: fadt
date: 2018-12-27
desc: How optional goals can conflict with the rest of your game
---
<h2>[The Anti-Pattern of Optional Goals in Tasklists](/blog/fadt/optionalGoals)</h2>

This may sound obvious, but if you give your players a goal, they will want to complete it. People want to complete everything that they can. This means that when you design a goal that is meant to be optional, you have to be careful with its implementation as players will default to trying to complete it, even if it is sub-optimal for them to do so.


Players want to empty tasklists. It feels satisfying to cross things off a todo list, whether in a game or not. That feeling of progress is something that many games use for a great deal of profit. For some games, the core loop revolves around this simple thing. A necessary consequence of this though is that leaving up goals that you do not intend for players to complete can be frustrating for players as they either live with the nagging itch of an unfinished tasklist or will spend effort and resources on a goal that does not provide a commensurate reward.

<img src="/blogImages/tqs_goal.png" />
## The Issue

It's worth taking a moment here to be clear about the exact issue that we're talking about. A lot of games feature explicit tasklists, such as quest logs or achievement screens. You can see these in games ranging from the grand strategy game *Stellaris* to an RPG like *Star Wars: Knights of the Old Republic* to mobile games like *Clash Royale* or even *Secret Passages: Hidden Objects*. Sometimes, games like these ones add optional goals to these lists. My argument is that the optionality of the quests can conflict with the tasklist.


If a goal is to be optional, then that optionality should be meaningful. If all of your players choose to complete an optional goal then making it optional holds very little meaning and if none of your players attempt it, then there is only rarely a good reason for it to exist. For an optional goal to be meaningful, there should be situations in which a player should complete them and situations in which a player should not. The decision to attempt the goal needs to be meaningful.


In something like *Knights of the Old Republic* for instance, I assume that I'll end up completing everything in my quest log before I leave the planet. Here, the quest log is a checklist that the players go through. As a result of this, this system trains players not to think about adopting quests, but just to do all of them. Thus, the player does not have to think about what to do next as the tasklist provides a clear and correct direction.


These two points conflict with each other, and so having both features in your game results in some dissonance in your design. The results of this can be:
- Players feeling frustrated that they cannot complete the game or that there is content that they are missing. Here, the first feature overpowers the second, so you get the benefits of the interesting decisions of which goals to pursue, but you lose the advantages of the second feature of a clear tasklist for players to follow.
- Players not engaging with the decision of whether to take up a goal, but simply doing all of them automatically. In this case, the second feature drowns out the first and you get the opposite of the previous case.



This tension between competing features in a single game tends to result in one of them ending up dominant causing the other to lose much of its benefits and the player to experience frustration from the dissonance.

## The Quiet Sleep

This note was prompted by an issue I saw in my own game *The Quiet Sleep* ([coming soon on Steam](http://store.steampowered.com/app/724510/The_Quiet_Sleep/)). The game used to have all of the goals appear on the map directly and the player would progress through the story through the completion of these goals. It was difficult to design in narrative choices as a result of this because the players would just complete all of the goals that appeared in front of them. The core loop of the game involved completing most of the goals that appeared and so it was difficult to explain that some goals were not necessarily meant to be completed.

<img src="/blogImages/tqs_goalMenu.png" />

To fix this, I added a step for these goals and made the player build the goals that are optional before they can be completed. The action of building a goal requires will, a currency that the player is typically short of, and is similar to building a tower. By doing this, the player is asked whether they want to make this goal more than any of the other things they could be doing with the will and so the player naturally applies critical thought to the goal. Note though, that by doing this the game no longer really has a clear tasklist and so it is easier for players to lose track of what they were doing and what they should do next. The optionality of some goals is key to the game, and so I chose it over the clarity of the tasklist.

