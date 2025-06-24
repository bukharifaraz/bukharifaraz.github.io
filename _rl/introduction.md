---
layout: single
title:  "Introduction"
classes: wide
date:   2025-05-16 13:32:01 +0530
categories: RL ML AI
tags: RL
---

<h3>Sequential Decision Making</h3>
<p>There are many tasks in which an agent needs to <u>"sequentially" decide</u> which one of the many possible actions it should take. For example consider the following <b>cliff-problem</b>:</p>

<img src="/assets/rl_images/intro_cliff_grid.gif" alt="Grid with Cliff" />

<p>There is a 4x12 grid.  The task is simple: the agent (that little elf-looking guy) needs to move from the starting point at [3, 0] to the goal at [3, 11] without falling off the cliff.</p>

<p> Clearly, to solve the challenge, the agent must "decide" at each step "which one direction to move in" out of all possible directions. The sequence formed by the directions chosen by the agent at each step, during its journey from initial to final position, constitutes a solution path. Obviously, there can be many such solution-paths (all not necessarily optimal[1]) One such path is shown below: </p>

<img src="/assets/rl_images/intro_cliff_grid_soln.gif" alt="Solution" />

<p>We use Reinforcement Learning to solve such kind of 'sequential decision making' problems.</p>





<div>[1]: optimality can be defined in different ways like least time taken, least steps taken, farthest from the cliff etc.</div>
