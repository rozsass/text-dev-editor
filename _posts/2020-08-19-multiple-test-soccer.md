---
title: 'Goalkeepers, random play and multiple testing'
date: 2020-07-18
permalink: /posts/2020/07/multiple-test-soccer/
tags:
  - multiple test
  - ch06
  - methods
  - football

---

Random action may be a well thought out strategy. Sometimes you would want to act randomly to make your next action hard to predict. This is particularly important when there is an adverserial situation, and players must choose a strategy. In game theory, this idea of picking an action from a set randomly is called [mixed stratgy](https://en.wikipedia.org/wiki/Strategy_(game_theory)) One such case is saving penalties. 

How can we test if goalkeepers play mixed strategies? Well, we can test if they move randomly, and test randomness for a large set of goalkeepers. 


## Stats and the beautiful game

Testing the hypothesis of random action across goalkeepers is what  Ignacio Palacios-Huerta carried out in his wonderful book ([Beautiful Game Theory: How Soccer Can Help Economics](https://press.princeton.edu/books/paperback/9780691169255/beautiful-game-theory). 


 ![image](/images/messi_penalty_kick2.jpg){: style="float: left"}

In the very first chapter, the author looked at penalties, from the point of view of randomness. Goalkeepers often decide to move before the ball is shot. Having collected data on where the goalkeeper moved, he tests if moves (such as left and up or right and  down) are random. Random action is mixed strategy. For 40 keepers, two of them are found to have non-random system of moving at 5%. This is exactly the number of falsely accepted $H_{A}$, we would expect based on chance. 

Thus, finding two keepers not seemingly follow random action does not indeed prove that the do not play mixed strategy. Instead it shows, that for multiple testing, we should need a tigher confidence interval, maybe 1% or 0.05%. With such a tight CI set for multiple testing, we could not reject random action for either goalkeeper. 

# reference
[Image](https://commons.wikimedia.org/wiki/File:FWC_2018_-_Group_D_-_ARG_v_ISL_-_Messi_penalty_kick.jpg)