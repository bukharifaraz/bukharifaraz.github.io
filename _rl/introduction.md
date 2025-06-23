---
layout: single
title:  "Introduction"
classes: wide
date:   2025-05-16 13:32:01 +0530
categories: RL ML AI
tags: RL
---

<h3>Sequential Decision Making</h3>
<p>There are many situations in which an agent needs to decide which one of the many possible actions it should take. For example consider the following problem:</p>

<img src="/assets/rl_images/intro_cliff_grid.gif" alt="Grid with Cliff" />

<p>There is a 4x12 grid.  The challenge is simple: the agent (that little elf-looking guy) needs to move from the starting point at [3, 0] to the goal at [3, 11] without falling off the cliff. The agent further has to ensure that it complets the challenge in the minimum amount of steps.</p>

<p> Clearly, to solve the challenge, the agent must decide at each step which direction to move in. Obviously, there are many such paths (all not necessarily optimal) which will take the agent from its inital position to the required destination. </p>

<img src="/assets/rl_images/intro_cliff_grid_soln.gif" alt="Solution" />







