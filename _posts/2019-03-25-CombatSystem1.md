---
layout: post
title:  "First Post: Quick Overview of the Combat System."
categories: [Combat,Systems]
tags: [overview,combat,systems]
---

The philosophy of this project is not to simulate a real combat, but to model it. The diference is that the focus will not be to get an accurate 'how' the action goes, but an accurate 'outcome' of the battle. To achieve this we will use the concept of _theatLevel_. This(ese) parameter(s) will be defined as a function of how dangerous is to be in a zone of the battlefield. It will dertemine the probability of damaging/disabling/killing an unit in that area, and will also determine the behaivouis of the units on the area,  thorug a filter called _threatPerception_.

To simplify let us assume that there is only one threat source, for exampla an infantry fire team covering from zone B a zone A. Supose that this gives the area A a treatLevel 0.5. This will mean that every action (take cove, fire, move, aid a fellow soldier..., I know is hight, the fire team is armed with PKM over open field) will be threatened with a probability of 1/2 of killing another infantry unit in zone A. This infantry threatened infantry unity will do 2 checks, a morality check against theri percieved threat (function of the diverse threats) and a survival check, done against the real threat (also function of threat on the area, and internal (camuflage, kevlar, ceramics ...) and enviromental (terain, fox-hole, woods, rain ...) factors that modifye the treats) 

In the following posts I will detail the iner workings of this model.