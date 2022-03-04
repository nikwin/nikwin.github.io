---
layout: post
title: The Quiet Sleep: Mechanical Parallels
tag: city
date: 2018-12-24
desc: A deep dive into an interesting design approach
---

<p style="font-size:10px">Written: 2017-08-12


As I wrote about in [my previous post](/blog/city/flip), I want this third story to explore where the mechanics can take this game. Historically, the story aspect had dominated the pieces that I've built, so I decided to design a few units and towers as though the game had a more standard military theme, and see what came of that.

## Units

A quick pass on the units for a tower defense gave me this:
  <table border="1" cellpadding="2">
    <tr><th>name</th><th>number</th><th>type</th><th>health</th><th>speed</th></tr>
    <tr><td>soldier</td><td>3</td><td>bio</td><td>1</td><td>5</td></tr>
    <tr><td>drone</td><td>3</td><td>mech</td><td>1</td><td>5</td></tr>
    <tr><td>tank / shielded tripod</td><td>1</td><td>mech</td><td>3</td><td>3</td></tr>
    <tr><td>brute</td><td>1</td><td>bio</td><td>3</td><td>3</td></tr>
    <tr><td>thor</td><td>1</td><td>mech</td><td>5</td><td>2</td></tr>
    <tr><td>giant</td><td>1</td><td>bio</td><td>5</td><td>1</td></tr>
    <tr><td>flight</td><td>5</td><td>mech</td><td>1</td><td>5</td></tr>
    <tr><td>swarm</td><td>5</td><td>bio</td><td>1</td><td>5</td></tr>
</table>


Note that:
- There's no alternate movement pattern. Many tower defense games put in things like flying units or tunneling units or something similar that forces the player to consider multiple angles of attack when setting up their defenses. I think the game manages to keep the decisions of what towers to build and where to build them interesting without wrinkles like this, so I'm just going to leave them out.
- There are no weapons on the units. While I think that having parts of your mind get destroyed by emotion would be strong storytelling, I don't want to introduce the complexity associated with that feature to my game. I feel like the current paradigm of having towers deplete holds much of the same storytelling, but plays better.



From this, we can see that the units break down across two axes:
- Type: *bio* or *mech*
- Number / health / speed - *3/1/5* or *1/3/3* or *1/5/2* or *5/1/5*



By this, we're making a bunch of archetypes for number, health and speed and making sure that our units fall into those buckets. We're also treating cost as a dependent variable, and so calculating it based off the unit's other attributes. As we only have two sliders, there are only 8 possible units from these parameters and those are the ones listed above.

## Towers

Similarly, a quick pass on the towers gave me this:
  <table border="1" cellpadding="2">
    <tr><th>name</th><th>shoots</th><th>splash</th><th>damage</th><th>rate of fire</th></tr>
    <tr><td>machine gun</td><td>bio</td><td>no</td><td>1</td><td>5</td></tr>
    <tr><td>bunker</td><td>bio</td><td>no</td><td>1</td><td>3</td></tr>
    <tr><td>turbolaser</td><td>mech</td><td>no</td><td>5</td><td>1</td></tr>
    <tr><td>gas bomb</td><td>bio</td><td>yes</td><td>3</td><td>1</td></tr>
    <tr><td>ion burst</td><td>mech</td><td>yes</td><td>3</td><td>1</td></tr>
    <tr><td>cannon</td><td>mech</td><td>no</td><td>3</td><td>3</td></tr>
    <tr><td>neural disruptor</td><td>bio</td><td>no</td><td>5</td><td>1</td></tr>
</table>


This gives us these axes:
- Shoots: *bio* or *mech*
- Splash: *yes* or *no*
- Damage: *1* or *3* or *5*
- Rate of fire: *1* or *3* or *5*



This gives us 36 possible towers, which is more than we probably need. I'll return to this later though.

## The Question of Pre-Made Units

At this point, it looked like I had a major decision to make - should the units be pre-made or should I just allow the players to make their own combinations of attributes?


I feel that designer-made units are going to lead to more interesting gameplay than allowing players to build their own units because it lets the players crystallize their decision of which tower to make around which units the opponent is likely to play.


An example of what I mean would be a player that has a bunker and a turbolaser from the above table. So, the defense is prepared for a swarm of bio units or a large mech unit. I feel like if the units are procedural, then the defending player is going to decompose their defense into the component parts and see that they have 1 point of defense against the 4 options of swarm, single unit, bio and mech and then shore up the defense against the permutations that are not explicitly addressed, like large bio units. What I want them to do is look at their defenses and see that nothing defends well against the giant. It's a nuanced difference, but I think the latter is better gameplay.


This means that I won't put in all the permutations and that the units are going to be spread out across a variety of buildings, so as to emphasize their uniqueness.

## Units 2

For the second iteration of the units, I wanted to change away from bio as a type because I didn't like how that would fit into the economy, so I changed the axes to:
- Armor - *physical* or *energy*
- Size/number - *3 small guys* or *1 medium guy* or *1 big guy* or *5 small guys* or *3 med guys*



From this, we can imagine construction options like:
- Barracks
- Drone bay
- Construction bay
- Brood pod
- Mass factory


## Buildings 2

From the changes to units, I reduced the axes for buildings to:
- Ammunition: *physical* or *energy*
- Splash damage: *yes* or *no*
- Damage/rate of fire: *1/3* or *1/5* or *3/3* or *3/1* or *5/1*



Construction options:
- Armory
- Synthesizer
- Gas Producer
- Inductor


## Further Notes
- I think a clever thing would be to allow people to build armor and a chassis and then put them together to make units. They should be multi-step goals that you can finish in multiple ways.
- I want to have both emotions that you can craft and send at your opponent and ones that come up more naturally.
- Note that the armor for the units and the ammo for the towers use the same raw materials.
- You should still need the right construction building for the units that you want to build.


## Creeps

This is where I started the process of converting from the soft science fiction of the units to the emotions of the creeps of *The Quiet Sleep*.


The types *anger* or *sadness* or *joy* work well as a direct parallel to the *physical* or *energy* of the units. These need raw materials like the *energy* and *metal* that the units above would have needed.

## What is the kind of event that would be a lot of small pieces?

  <li>joy:
- Hobbies - like fishing or playing video games. These may by better as calming influences though. I very rarely feel overwhelmed with joy from these, I just feel in a good mood.
- Reading/hearing compliments.
- Having a good conversation.
  </li>
  <li>anger:
- Having a bad/boring/dull/gauche/unintelligent conversation.
- A series of interruptions when in flow.
  </li>
  <li>sadness:
- Hearing criticisms.
  </li>

## What would be the cause of a large emotion?

  <li>joy:
- Taking a major career step.
  </li>
- anger:
  <li>sadness:
- The death of a dream.
  </li>

## What are medium things?

  <li>joy:
- Work going well.
- Compliments from someone respected.
- Giving in to a vice - something like my going to music shows.
  </li>
  <li>anger:
- Being stuck with work.
- Dealing with something stupid.
- Noise when you want silence to focus - being in a mood where you want to be left alone to focus and not being able to get that space.
- Feeling like you're not getting work done.
  </li>
  <li>sadness:
- Work going poorly.
- Crisis of faith.
- Flashbacks to old pain.
- Feeling alone.
  </li>

## Creeps 2

We can reduce the above to the following methods of delivery:
- Lots of small comments - 3 creeps, 1 health, 5 speed
- Upgraded small comments - 5 creeps, 1 health, 5 speed
- Flat statement - 1 creep, 3 health, 3 speed
- Major statement - 1 creep, 5 health, 1 speed




  <table border="1" cellpadding="2">
    <tr><th>topic</th><th>type</th><th>small</th><th>flat</th><th>major</th></tr>
    <tr><td>compliment</td><td>joy</td><td>X</td><td>X</td><td></td></tr>
    <tr><td>criticisms</td><td>sad</td><td>X</td><td>X</td><td></td></tr>
    <tr><td>interruptions</td><td>anger</td><td>X</td><td></td><td></td></tr>
    <tr><td>work going well</td><td>joy</td><td>X</td><td>X</td><td></td></tr>
    <tr><td>giving in to vice</td><td>joy</td><td></td><td>X</td><td></td></tr>
    <tr><td>stuck with work</td><td>anger</td><td>-</td><td>X</td><td></td></tr>
    <tr><td>slow work</td><td>anger</td><td>-</td><td>X</td><td></td></tr>
    <tr><td>stupidity</td><td>anger</td><td>X</td><td>X</td><td></td></tr>
    <tr><td>feeling alone</td><td>sad</td><td>-</td><td>X</td><td></td></tr>
    <tr><td>poor work</td><td>sad</td><td>X</td><td>X</td><td></td></tr>
    <tr><td>old failures</td><td>sad</td><td>X</td><td>X</td><td></td></tr>
    <tr><td>crisis of faith</td><td>sad</td><td>X</td><td>X</td><td></td></tr>
    <tr><td>death of dream</td><td>sad</td><td></td><td></td><td>X</td></tr>
    <tr><td>major career step</td><td>joy</td><td></td><td></td><td>X</td></tr>
  </table>


## Creeps 3


    <li>Standard topics (can deliver as small or flat):
- Compliments - joy
- Criticisms - sadness
- Feeling alone - sadness
- Old failures - sadness
- Slow going with work - anger
    </li>
    <li>Additional:
- Vice - joy, flat
- Stupidity of others - anger, flat
    </li>
    <li>Major points:
- Death of the dream - sadness
- Major step in work - joy
    </li>
    <li>Game events:
- Interruptions - anger, small
- Boosts for: compliments, criticisms, old failures, vice, stupidity of others
    </li>


## Notes on Emotions
- Make the opponent very good at nullifying joy. It makes for good storytelling.

## Towers
- Types: *anti-anger/sadness* or *anti-joy* or *anti-all*.
- Rate of fire: *slow* or *fast*



I decided to take out splash as it plays equivalent to a fast rate of fire and to make damage a dependent variable on rate of fire.



<table border="1" cellpadding="2">
  <tr><th>name</th><th>type</th><th>rate of fire</th><th>notes</th></tr>
  <tr><td>Support</td><td>anti-negative</td><td>fast</td><td></td></tr>
  <tr><td>Keeping Busy</td><td>anti-negative</td><td>slow</td><td>I'm never able to focus on work when I'm feeling happy.</td></tr>
  <tr><td>Toughness</td><td>anti-all</td><td>fast</td<td></td></tr>
  <tr><td>Calmness</td><td>anti-all</td><td>slow</td><td>We need this to be distinct from toughness because the opponent needs strong defenses</td></tr>
  <tr><td>Sharing Joy</td><td>anti-joy</td><td>fast</td><td></td></tr>
  <tr><td>Mistrust of Joy</td><td>anti-joy</td><td>slow</td><td></td></tr>
</table>



These are the towers for the opponent and I might have to build in more of them or some upgrade trees for them if they feel too flat, but we'll first take a look at how this plays before planning out extensions.


Also, this doesn't cover the towers for the player character in the game. I want to share as many towers as I can between the PC and the antagonist, so we'll see how that works out too.

## Tasklist

From this document, I can derive the following tasklist:
- Figure out the steps to make a unit or a tower from this
- Work out this part of the economy
- Implement nine creeps
- Implement seven game events
- Implement six towers
- Try to make it so that the PC can also access these towers
- Make sure to support the different parameters for creeps
- Make sure to support the different parameters for towers



From here, all that's left is the implementation of these pieces and some playtesting to see how things play together.

