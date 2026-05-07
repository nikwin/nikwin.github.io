---
layout: post
title: "Mechanical Foreshadowing"
tag: fadt
date: 2018-12-21
desc: "Going over what mechanical foreshadowing is and how to integrate it."
---

*(Not sure what FADTs are? Read about them [here](http://www.gamasutra.com/view/feature/3357/formal_abstract_design_tools.php))*

Foreshadowing is an important and commonly used narrative device that indicates what is to come so as to build anticipation and make twists more believable. The mechanical equivalent of this is actually fairly common in video games as well. With this article, I'm going to break down the pieces of this mechanical foreshadowing, list some of its advantages and disadvantages, and go over possible variations of its base formula.

## Hookshot of Zelda
![Zelda hookshot image](/blogImages/hookshot.png)

Let's use the case of the hookshot in *The Legend of Zelda: A Link to the Past*. The game shows you places where you can use the hookshot long before you actually get the item. So, when you finally get the hookshot, you know of a number of places where you can use it and you have an idea of what it does.

## Advantages

Mechanical foreshadowing of this nature has a number of advantages when compared to simply introducing the item and only then introducing its uses. They are:
- **Rewards feel more valuable** - Now, when you get something new, it not only holds its intrinsic value, but it also holds the value of the things that are now unlocked.
- **Changes the reward cadence** - By structuring your rewards like this, the point where the player understands the reward is brought much closer to the point of getting the reward. This makes the reward itself significantly more impactful. Often, when the player gets a complex new piece as a reward, the feeling of being rewarded is eclipsed by puzzlement at what exactly this new thing can do. By having already shown the player some uses of this new item, that puzzlement is obviated.
- **Integrates better** - The real world does not wait for you to obtain the tools to solve a puzzle before presenting you with it. Video games often do so as a concession to playability, but interleaving obstacles and tools more naturally helps the game world feel believable. Additionally, it works effectively as a way to gate players from more advanced sections of a game.
- **Raw fun** - It's very empowering in a game to be able to overcome obstacles that earlier stymied me. Presenting the problems to players before they can solve them makes that moment of being able to solve them feel like a real level up. Additionally, it is satisfying to be able to use things that you could not before.
- **Indicates depth** - By placing insoluble problems early on, the game piques the player's curiosity and lets them know that the game is going to get wider before actually widening the game. Thus, as a designer, you can run a slower complexity curve without worrying that the player will prematurely dismiss the game as shallow.
- **Anticipation** - Showing players potential rewards early builds up a sense of anticipation for when the player can actually use them.


## Requirements

So, now say that you want to thread mechanical foreshadowing into your game, what would you need?
- **Something to foreshadow** - You need something that mechanically changes or expands the game for you to foreshadow.
- **Locks or requirements** - You need some obstacle preventing the player from just immediately getting the tool to solve the problem that is foreshadowed.
- **Non-linearity** - Players need to be able to return to things that they have encountered previously so as to convert the foreshadowing event.


## Risks

Like most patterns, there are risks associated with this one and it is dangerous to apply it blindly.
- **Clarity** - It needs to be clear to players that they don't have the tools to solve a problem when they first face it. It's pretty clear that the player cannot make their way across the gap with the tools that they have available in the *Zelda* example above. However, if your double jump doesn’t go that much further than your single jump, you’re going to have players trying to jump a gap that they cannot manage because they don't know how else the game expects them to cross.
- **Keeping old problems in mind** - If the player has completely forgotten about the foreshadowing event when they get the new tool, the result is slightly worse than if you did not foreshadow at all. You've spent effort to present the player with an insoluble problem. Ask yourself is the kind of game where players would have the time and spare focus to notice the foreshadowing and whether it’s the kind of game that encourages players to think back on past events. Open world games, like *Zelda* do well on both these axes, but yours might not.
- **Complexity** - This foreshadowing adds a complexity hit to the player, and does so before it would have been necessary otherwise. Complexity curves are unsurprisingly complex and this adds a wrinkle to an already difficult problem.
- **Resentment** - If your foreshadowing is too obvious and held off for too long, your players may start feeling resentment. You can especially see this with quality of life upgrades, like double jumping, sprinting and fast travel. Like with narrative foreshadowing, this is best when only obvious in hindsight. *(Thanks to [@merusworks](https://twitter.com/merusworks) for pointing this out.)*


## More examples

- **Locks and keys** - The original *DOOM* is famous for this. Presenting the lock before the key works much better than the other way around. If you’re going to put the lock after the key, you may as well skip both. This is a base case for the foreshadowing pattern as a whole, and as such isn’t that good an example. As the key lacks any kind of mechanical value beyond being a key, the player cannot get excited about it and the possibilities that it opens up. As such, this plays more like a wrinkle of the level design than of the reward cadence.
- **Tool upgrades in *Stardew Valley*** - This implementation of the pattern is also fairly straightforward. The game has logs that are too hard for your starting axe and stones too tough for your early pickaxe. There are some of both right outside your house and you can't help but to encounter them right at the beginning of the game. This works better than the previous example because the upgrades have more gameplay significance and the upgrade tree is a fundamental motivation in the game.
    ![Stardew Valley image](/blogImages/stardew.png)
- **Playing against cards** - In a game like *Hearthstone*, you often play against a card before you actually own it. Thus, when you finally pick up that rare, you have a solid idea of what you want to do with it.
- **Visiting other farms** - A game like *Farmville* does almost exactly the same thing as the previous example by pushing people to visit other people's farms. This way, players get exposure to content well before they get it and so can figure out what they want and anticipate that.
- **Water in *Civilization*** - Seeing land across water in 4X games like *Civ* works out very cleanly to a form of mechanical foreshadowing. It's clear that you can't cross the water yet, but that you will be able to. So, when you gain the ability to build boats, you already have some idea of what to do with the new ability and where you want to expand to next.
    ![Civ 6 water image](/blogImages/civ6_water.jpg)
- **RTS tech trees** - Building something like the barracks in *Starcraft* will show you a list of units, many of which are locked until you build a specific building. This feels closer to mini-goals than to mechanical foreshadowing though due to the optionality of building tech buildings. Additionally, the repetition of coming across this every time you start a new skirmish takes away from the feeling of foreshadowing.

## Possible Variations

When looking at the mechanic from this angle, we can imagine variations that explore the core idea a little more.
- **Blight** - Imagine having a spell in an ARPG-style game that is powerful, so the player naturally uses it regularly, but which fails sometimes in areas where the blight has spread. Then, when the blight takes over the world in the second act, have the ability always fail. Thus, when the major narrative twist of being unable to prevent that blight happens, it has gameplay effects as well that the mechanics have foreshadowed.
- **Character Sickness** - Similarly, having a character be occasionally unavailable due to sickness foreshadows that character eventually succumbing to that sickness both mechanically and narratively.
- Note that both of these are the inverse of the examples presented above as they deal with removing a piece, not adding one. So, naturally all of the advantages listed above aren't all applicable, but the experience would flow better than simply removing the piece.
- **Town Happiness** - You can imagine an RTS that starts with setting up a settlement to produce war materiel, but which occasionally tasks you with keeping the population of your town happy. Then, when peace comes, the game transitions into just being a city-building game.
- **Trading** - We could have a dating game in which you're trying to put together enough money to buy presents for the person that you're trying to impress and you get (in-game) happiness from making good deals. Then, when the game drops the twist of having the person that you're trying to impress drop you for shallowness and has the player character find out that what they really love is making money, the twist has had mechanical foreshadowing as well.

## Conclusion

Mechanical foreshadowing is a design tool that can be used in a wide variety of games and should help with reward cadences and the impact of twists in your game. Hopefully this article has helped you figure out if it will work for your game and how you can integrate it.

