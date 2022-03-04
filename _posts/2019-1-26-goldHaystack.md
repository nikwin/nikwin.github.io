---
layout: post
title: Gold In The Haystack
tag: fadt
date: 2019-1-26
desc: How to seed info dumps with approachable elements.
---
<h2>[FADT: Gold In The Haystack](/blog/fadt/goldHaystack)</h2>

*(Not sure what FADTs are? Read about them [here](http://www.gamasutra.com/view/feature/3357/formal_abstract_design_tools.php))*


A number of games task the player with choosing a subset of a large group of linked items, such as building a deck out of a collection of cards. This is often difficult for newer players to engage with because of the high frontloaded complexity of being presented with the full set of items.


Choosing a few core elements can make the process of choosing the rest of the elements much simpler for the player. So, designing such that players can easily determine that core makes the process of choosing the full subset much easier.

## Example - Sealed in *Magic: the Gathering*
<img src="/blogImages/callOfTheConclave.jpg" />

Take the example of sealed deck in *Magic: the Gathering*. In this format, every player gets six unopened packs which translates to 90 cards out of which they need to make a deck of 40 cards, about 17 of which will be basic lands that come from outside the pack.For a new player, the challenge of understanding all 90 of the freshly opened cards and comparing between them is quite forbidding.


However, only six of these cards are rare or mythic rare and the idea of rare cards being better is an easy one for new players to grok and the rare cards are typically the most eye-catching ones anyway. Choosing which of those cards to play with is a much more approachable decision for a new player. Once the player has chosen the core of the deck like this, they are able to choose the colors and style of deck that they want to play and so filter down the set of cards by a large factor.


Thus, designing around giving players an easy starting point for the complex, compound decision of what deck to make can drastically simplify the process for new players.

## Requirements
- <b>Requiring the player to choose a subset of a large group of items</b> - Stuff like deck building or choosing an upgrade from a large tech tree or choosing what all to build with limited resources all require the player to choose a subset from a large group of items.
- <b>Links between elements</b> - For *Magic: the Gathering*, the colors provide a direct link between the core cards chosen and the rest of the deck. Additionally, the core often defines the style of the deck, which provides another way to filter which cards to add to the deck. Without this, you may have players easily determine the first five items of the set but be completely stuck with the next twenty.
- <b>A simple filter to determine core options</b> - Players need an easy way to determine which elements are possible choices for the core. In *M:tG*, the rarity is easy to understand and something that new players naturally gravitate to. Note that this wouldn't work well if the rare cards weren't also clearly better than the non-rare cards.
- <b>A strong filter</b> - This first filter also needs to remove most of the options. Here, the player goes from 90 options to 6 options, which is a very manageable number. If you have something like 24 options instead, then that first decision is still going to be too complex for your players.

## Effects
- <b>Reduced complexity for new players</b> - This is the reason for the FADT and the most important consequence of its implementation. The importance of making your game approachable to new players cannot be overstated.
- <b>Reduced depth overall</b> - It's possible that this is avoidable, but having a smaller set of options for a core does reduce the size of the possibility space for your game, and so reduces depth.
- <b>Fine-turning</b> - The size of the subset generated gives the designer another knob to use to fine-tune the depth and complexity for newer players.

## More Examples
<img src="/blogImages/civTech2.png" />
- <b>Deckbuilding in *Hearthstone*</b> - This is pretty obvious, but deckbuilding in *Hearthstone* follows the same FADT. There are a few cards from every set that stand out and people start by building decks around them instead of trying to solve the whole set at once.
- <b>Upgrade trees</b> - Trying to figure out a path through an upgrade tree is another instance of trying to choose a subset of a large group of items and similarly struggles with frontloaded complexity. Separating the tree into schools grouped thematically in a way that the player can understand really reduces their effective complexity.
- <b>The tech tree in *Civilization*</b> - The tech tree in a game like *Civ* is massive and sprawling. The complexity is mostly mitigated by presenting the short term choice of what to research next, but when you're looking for longer term plans, the game has certain things like districts and governments which the player can zero in on.

## Further Thinking
## Netdecking

The classic solution to problems like this is to netdeck. It's very easy now to just go online to figure out good decks or good builds and just copy them directly. This is functionally equivalent to taking out most of that aspect of the game and so this FADT may be partially obsolete now unless used for something that provides randomly generated challenges, like sealed deck in *M:tG*.

## Inherent Difficulty

Even with this FADT, the task is likely to still be difficult. New players often ask for lots of help when building sealed decks because it is still quite challenging to make a deck from a set of cards that you don't understand, rarity filters or no. Complexity hits like this are always going to be difficult for players to manage and there's only so much that you can do as a designer to mitigate that difficulty.

