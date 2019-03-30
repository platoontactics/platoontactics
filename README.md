---   
layout: page
---
# PlatoonTactics

## Introductions

*PlatoonTactics* is a a top down 2-D RTS game where you make you battle plan and play it out, perceiving the combat through updates of your troops, and issuing new orders to adapt to the shifting environment and overcome your enemy. Become a combat leader and me use of your best tools: a map, radio and your wits.


## Description

The objective of this game is to model how a battle would go in squads and platoons, units  under company level, what is know as [small unit tactics](https://en.wikipedia.org/wiki/Small_unit_tactics) . The player will be able to make a combat plan over a map, with [tactical markings](https://en.wikipedia.org/wiki/NATO_Joint_Military_Symbology), to accomplish a task set by its commanders, like defend a hill, assault a bunker, provide cover to a marching battalion, patrol a large area ... The units available and the time to prepare the plan will depend on the scenario.

The enemy will have its own plans and objectives, usually opposing to that of the player. When the planing time is up, the units will act according to the given orders, and engage in combat. In this phase of the game, the player will not be able to micromanage the units, but they will obey new orders, in the degree that they are able. The information will be conveyed to the player through status reports of the units and updates on the tactical map, with signgtings, engagement, movements of troops. The player will not have total information of the situation, and what it has might be outdated if he hasn't received reports form his units.

As hinted before, the Graphical Interface will be the map with flags and markings for the units, arrows and lines to indicate movement and fire and other actions. The Interaction will be done constructing task orders from icons over the map, that might be detailed or general, and assigning the tasks to units. The map is to be updated periodically with information of relayed by the units back to the player, and will appear also as a text log.

## Features

 1. Game engine that models and displays the combat.
 5. Unit factory to design and deploy a variety of units and to the field.
 2. Order factory to make and distribute orders to the units involved.
 4. Actor AI to give autonomy while carrying out orders to the units and make them effective on combat and react to the situations.
 3. Enemy planer AI to pose a challenge to the player.
 5. Simple and sober UI based on vector graphics over realistic maps.

## Implementation

As this is a learning experience, as much as possible will be home-brew, making the game engine with Entity-Component-System paradigm, to learn what is has to offer, and because I **believe** that it will offer more flexibility down the line to add features. The language of choice will be C++, as it has ubiquity everywhere and usable with lots of libraries.

Things that can "externaled" to a library can be the the user interaction (graphics, input and GUI). This is to be determined, but open-source should be always choosen over propetary.


## Road Map

1. (Ongoing) Design the **combat system** based on threatLevels.
3. Design of the **units**, as aglamation of components.
4. Design the environment and how it affects the combat and units, and how it is affected by them.
2. Implementation of first iteration of the **combat system** taking into account the previous points.
5. Design and implementation of the **Unit AI**
6. Testing and geting a feling of the game so far.
7. Re-think points 1-4 with new insights.
8. Design the **order factory** and adapt the **Unit AI** to it.
9. Heavy playtesting different scenarios with given orders.
