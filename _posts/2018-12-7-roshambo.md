---
layout: post
title: "On Rock, Paper, Scissors"
tag: articles
date: 2018-12-7
desc: Examining some of the features of rock, paper, scissors.
---


*Rock, Paper, Scissors* is ubiquitous. Most people (and even some [lizards](https://en.wikipedia.org/wiki/Common_side-blotched_lizard#Mating)) have played it at some point. Additionally, many larger games use systems based on it. It's also a fairly interesting case study for a number of interesting design principles, so let's take a look at those.

## The Importance of Framing

It's hard for people to have fun in places that they don't expect to find fun. Framing a repetitive task as a challenge to improve at is a tried and true way to make that task more fun.

<img src="/blogImages/coin.jpeg">

With *Rock, Paper, Scissors*, people often frame it as a random and fair way to make a decision, much like flipping a coin. Viewing the game from this perspective leads to two interesting insights. The first is that giving people some autonomy in a random decision helps improve the experience of that randomness. It lets you believe that you can do better the next time if you lose and lets you feel proud of your skill if you win. This is why choosing when to stop a spinning wheel is more fun that just watching it go.


The second piece is that if I am to look at *Rock, Paper, Scissors* as an RNG, then trying to work out the optimal play is sort of like cheating. Choosing which move to make could be an interesting decision for many people, but viewing it as an interesting decision is against the point of the game. Also, as it is normally played, people do not really have the time to work out a move. The game is over before a mind can switch gears into figuring out what to play.

## Gameplay

Despite the fact that there are a lot of games that use a core of *Rock, Paper, Scissors* to great effect, I think that the base game itself is not that fun. These systems allow players to exercise yomi, or the ability to read the minds of their opponents, in the game. However, I think that when stripped down to pure *Rock, Paper, Scissors*, it cannot support this skill for the following reasons

## The Decision of What To Play

A problem with a decision that is purely symmetric in the manner of *Rock, Paper, Scissors*, where rock, paper and scissors are functionally identical is that there is no real starting point for the player to use when making this decision. There's no mechanical advantage or even difference to all of them, so the player cannot frame their decision in the mechanics of the game. Additionally, there's no semantic difference between the three options so people cannot bring their own preferences in either. I imagine if the game was called love-hate-reason instead, players would find it easier to make a decision about what to play.


As players are often unable to make a real decision about what to play, people play rock and scissors more than paper as they are easier to get to from a last-moment closed fist. This fact actually makes for a reasonable starting point on what you should play. Given just this fact, rock seems ideal, but maybe your opponent knows this and will play paper, which means you should play scissors. However, if your opponent has gotten this far, you should really be the one to play paper. Through this, you can argue yourself into any of the three options and so the decision can become interesting. Additionally, playing multiple games consecutively ameliorates this problem.


Games that incorporate *Rock, Paper, Scissors* for decision making thus tend to have the different choices also differ on other axes, so that you can make the read based on what you believe to be your opponent's risk tolerence or aggressiveness or other similar characteristics.

## Solving Rock, Paper, Scissors

There exist very good players and computer algorithms that win far more than half their games by exploiting psychological tricks and standard human thought patterns. This would indicate that it is possible to be skilled at the game.


However, if you were to make a truly random move every time you play, your chance of winning is exactly 50% against every strategy your opponent can adopt. This means that we can derive a more complex strategy where we play a random move when the opponent is more skilled than we are and use our skill if they are less skilled than we are. This guarantees us a chance of winning greater than or equal to 50% against all opponents. However, our opponent can and should use this strategy as well. This means that our chance of winning is less than or equal to 50%. From this, we can see that if both players are playing optimally, one of them will make a random move resulting in both players having a 50% chance of winning. As this is true independent of the skill level in the game, it is clear that skill is not important when players are playing optimally. Hence, developing skill at this game does not provide a player with any return on the investment of time that player has made if everyone plays optimally.


Additionally, for any pointing of the different victory conditions that you set, it is trivial to derive a weighting of the options that will give you a 50% chance of winning. For instance, if a win with rock is worth twice as much as one with paper or scissors, playing 1/4 rock, 1/4 scissors and 1/2 paper will give you an E.V. of 0.


Note, of course, that if you remove a player's ability to determine how valuable each option is, you make it impossible for a player to determine the optimal strategy. Games with complex states, such as *Starcraft* or *Street Fighter* do this and so prevent their mindgames from being solved.

## Degenerate Solutions

The existence of a degenerate solution is not necessarily the death knell for a system. It only matters if your players believe it to be degenerate. Many games do very well despite degenerate systems because players finish the game before they solve the systems.


Also note that the game rewards skill until one player starts playing purely randomly. So, if a couple of people are just playing against each other and neither cares enough to work out how to solve the game, gaining skill in the game (by doing something like figuring out a pattern of play that your opponent uses) is rewarded by winning more.


While at first, it seems obvious that a game like *Rock, Paper, Scissors* would not be fun, the question of why is critical, especially given how simple the game is. I don't think that this article is exhaustive and I'd like to hear what other aspects of *Rock, Paper, Scissors* result in it generating the experience it does.

