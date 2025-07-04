---
layout: single
title:  "Introduction"
classes: wide
date:   2025-05-16 13:32:01 +0530
categories: RL ML AI
tags: RL
---

<hr>

<h3>Sequential Decision Making</h3>
<p>There are many tasks in which an agent needs to <u>"sequentially" decide</u> which one of the many possible actions it should take. For example consider the following <b>cliff-problem</b>:</p>

<img src="/assets/rl_images/intro_cliff_grid.gif" alt="Grid with Cliff" />

<p>There is a 4x12 grid.  The task is simple: the agent (that little elf-looking guy) needs to move from the starting point at [3, 0] to the goal at [3, 11] without falling off the cliff.</p>

<p> Clearly, to solve the challenge, the agent must "decide" at each step "which one direction to move in" out of all possible directions. The sequence formed by the directions chosen by the agent at each step, during its journey from initial to final position, constitutes a solution path. Obviously, there can be many such solution-paths (all not necessarily optimal[1]) One such path is shown below: </p>

<img src="/assets/rl_images/intro_cliff_grid_soln.gif" alt="Solution" />

<p>Reinforcement Learning is one way to solve such kind of 'sequential decision making' problems.</p>


<h3>Methods of Solving Sequential Decision Making Problems</h3>
<ol>
  <li>Explicit Programming</li>
  <li>Supervised learning</li>
  <li>Optimization</li>
  <li>Planning</li>
  <li>Reinforcement Learning</li>
</ol>

<h3>What is Reinforcement Learning (RL)?</h3>
<p>
  In the layman terms, RL is a way to learn sequential decision making using experience (or trial & error) 
 
</p>
<div>
   <u>RL has the following characteristics:</u>
<ul> 
  <li>No supervision is available to get the training. Learning happens via <u>trial & error</u>.  </li>
  <li>Decisions are to be taken one after the other. These are called '<u>sequential decisions</u>'. </li>
  <li>A decision taken in the very beginning can lead to a sub-optimal solution at the end. We call this as '<u>delayed reward</u>'. </li>
</ul>
</div>

<hr>
<div>[1] optimality can be defined in different ways like least time taken, least steps taken, farthest from the cliff etc.</div>
