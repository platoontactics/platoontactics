---
layout: post
title:  "Introduction to the Threat Levels I - Idea"
categories: [Design]
tags: [combat,systems,theratLevel,Idea]
excerpt_separator: <!--more-->
---


In this post we will overlay the idea of threat levels, and how they will effect the actors on this game. It abstracts the damage and psychological effects that a unit suffers by being on an area. This threat level is projected by other units to this area by diverse means.

<!--more-->

(*NOTE: This blog posts are to throw design and implementation thoughts to the air, and force myself to design instead of code, usually they come directly from some background aether infused with folk and celtic music.*)

## Description

Threat levels are a characteristic of the nodes. These levels are given by actions of different entities that target that node (or more, but this node is affected), for example opening fire, being armed on the node, mines, indirect fire ordinance, high caliber, perforating... 

These are given by actions of units and stored on nodes, after being modified by attributes of it, like cover, concealment. This will give the node *threatLevels* for each different type. On the other hand, the units in the node taking fire will perform two operations for with the threat level, one will be to asses their *percievedThreat* on the area, that will modify which actions they overtake, like taking cover, retreating, starting suppressive fire. This will be checked against a morale attribute and the *percievedThreat* will be fuzzy, in the sense that it my be off. 

The second operation is to figure out the actual threat that taking fire in that position entails and what effects will have on the unit. This might reduce the maximum firepower of the unit (representing lose of men - remember: model, no simulation), movement, morale, simultaneous actions..., the idea is gotten.


## What we take from here:


Enviromental entities, like nodes will have a component with the *threatLevels*, and those will be modified by the *FIRESYSTEM* looking over the *firePower* and *fireVector* of firing units. Thenn the *DAMAGESYSTEM* will update the units acord the *threatLevels* and internal componets of where they are and finally the  *AISYSTEM* would decide acording the *threatLevel* and the internal *behaivour* the next actions to take (this two systems could be reversed). 
