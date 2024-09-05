---
layout: post
title: Horticular's Overlapping Habitats
tag: fadt
date: 2024-09-05
desc: How the overlapping goals in Horticular lead to deep gameplay.
---

*Horticular*'s overlapping habitats make the game special. Every animal in the game has a habitat requirement. So, for example, a bumblebee needs a 5x5 space in which there are at least 5 flowers. A goldfish needs a habitat that's mostly water with some foliage and shading. The fun of the game is that it then follows that once you have a goldfish habitat, you can then very easily modify it to support bumblebees as well.

Overlapping goals is a very common pattern across games. Letting a player progress on a goal while completing a different goal is a fairly common pattern across games and adds a lot to the player's experience. *Horticular* implements this dynamic in a very clear, very skillful way and makes for a great example to use when breaking this pattern down.

## Advantages

- **Depth** - Overlapping goals gives players a lot of space to optimize and play more efficiently. It's fairly trivial to build a habitat for a single creature, but making it a habitat that can also support other animals takes a lot of thinking. This is very obvious when you look at the difference in thought between setting up a habitat in *Zoo Tycoon* which is a fenced off area for a single species and *Horticular* where it will overlap with multiple other creatures.
- **Flexibility** - This gives the player a sliding difficulty scale. If they feel like figuring out the optimal strategy that lets them complete the most goals in the fewest actions or space, then the game rewards them for it, but the game also allows them to solve different goals at different times. This might be less efficient but it still lets the player complete the challenges in front of them.

## Requirements

- **Goals**
- **Goals that can be completed with partial space**
- **Discrete cutoffs**
- **Overlapping spaces**
- **Items that do multiple things at once**

These become very easy to understand when you consider specifics. If a habitat has a fixed nine tiles that need to be filled with specific items, then there is no flexibility for the player to use to have another habitat overlap it. The goal needs to give the player scope to advance both it and another goal simultaneously. This is the same reason that the goals need discrete cutoffs. In *Horticular*, each habitat can support 1, 2 or 3 animals of that type. Practically, there is no difference between a habitat at 101% and 150%. If there were, then it would be natural for a player to build habitats that don't overlap in order to maximize the percentage of each of them. Similarly, if the habitats could not overlap, or if you can only progress a single goal at a time, like in *Zoo Tycoon*, then the solution becomes more rote as there's only a single set of requirements to solve.

It's also important to allow the player to make moves that advance multiple goals at once. *Horticular* has items that hit multiple categories at once. So, you can have a plant that counts towards the flowery requirements of the bumblebee and the foliage requirements of the frog at once. If each could only do one, then the problem of figuring out the perfect habitat becomes much easier.

## Risk

- **Burden of Optimal Play** - You need players to be able to accept sub-optimal solutions overall. Solving perfectly is much more complexity than is reasonable to expect from a player and so you need to be generous enough with constraints that players can achieve goals separately if need be.

## Variations

- **Modifying old solutions** - A very clever aspect of *Horticular* is that the habitats stay on the map as you unlock new creatures and items. So, you often find yourself looking through old habitats to see if a few small modifications can allow for more creatures in an already-existing space rather than needing to start from scratch for each new animal.

## B-Side

- **The organic of animals moving in** - Creatures in *Horticular* move in as they will and will also find habitats even if you haven't placed them. Choosing this instead of *Zoo Tycoon*-style purchase and zoning features adds something of the organic to the game.
- **Gardening** - However, the landscaping in *Horticular* is near absolute. You are able to change the terrain pretty much as you wish and the game starts as *terra nullius* with very little exception. You don't really have to negotiate at any point with the environment, but can instead just impose your will as you wish.