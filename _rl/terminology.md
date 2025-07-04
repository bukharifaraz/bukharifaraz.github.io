---
layout: single
title:  "Terminology"
classes: wide
date:   2025-05-24 13:32:01 +0530
categories: RL ML AI
tags: RL
---

<h3>Important Terms used in Reinforcement Learning:</h3>

<p>We will use the following cliff-problem which was mentioned in the <a href="https://bukharifaraz.github.io/rl/introduction/">introduction-post</a> to describe the important terms which are used throughout the RL course: </p>
<img src="/assets/rl_images/intro_cliff_grid.gif" alt="Grid with Cliff" />
<ol>
<li><b>Agent</b>
  <p>
     An agent is just something that acts <i>(agent comes from the Latin agere, to do)</i>. Of course, all computer programs do something, but computer agents are expected to do more: operate autonomously, perceive their environment, persist over a prolonged time period, adapt to change, and create and pursue goals. [1] 
  </p>
<p>
    In the context of RL, 'Agent is the "decision-maker" while solving a sequential decision making problem. It can also be called "learner" i.e. the one who learns to make sequential decisions. 
  </p>
<p style="color:green">
  In the cliff problem above, the little elf-like figure is the agent, as it makes a decision at each step regarding the direction in which to move.
</p>
  
  <p>
    A <b>rational agent</b> is one that acts so as to achieve the best outcome or, when there is uncertainty, the best expected outcome.
  </p>
</li>



<li><b>Environment</b>
  <p>
     The world with which the agent interacts.
  </p>
</li>


<li><b>State (s)</b>
  <p>
     The current situation of the agent/environment.
  </p>
</li>



<li><b>Action (a)</b>
  <p>
    The move the agent chooses.
  </p>
</li>





<li><b>Reward (r)</b>
  <p>
      Feedback signal for the agent’s action.
  </p>
</li>




<li><b>Policy (\(  \pi \) )</b>
  <p>
     The strategy the agent uses to decide actions.
  </p>
</li>





<li><b>Trajectory</b>
  <p>
     A sequence of states, actions, and rewards.
  </p>
</li>







  
</ol>

<div>
<h3>Interaction Cycle</h3>
<p>
Loop:
    Observe state \(s_t\)
    Choose action (a_t) based on policy π(s_t)
    Receive reward (r_t) and next state (s_{t+1}) from the environment
    Update policy to improve future decisions
  
</p>
  
</div>

<div>
  <h3>MDP</h3>
</div>

<hr>

<div>

  [1]: Artificial Intelligence: A Modern Approach (Russel & Norvig)
</div>
