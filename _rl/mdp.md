---
layout: single
title:  "Markov Decision Process (MDP)"
classes: wide
date:   2025-07-04 13:32:01 +0530
categories: RL ML AI
tags: RL
---

<hr>

<div>
<h3>Markov Process</h3>

A Markov Process is a type of stochastic process that satisfies the *Markov property* — the idea that the future state depends only on the current state, not the sequence of past states.


<h4>Layman Definition</h4>

In simple terms, a Markov Process is like a memoryless system:  Where you are now is all that matters in deciding where you go next. The path you took to reach here does not affect the next step.

<h4>Formal Definition</h4>

A Markov Process is defined as a tuple:

$$
(S, P)
$$

where:

- $$S$$ is a (finite or infinite) set of states. 
- $$P$$ is a transition probability function, such that:

$$
P(s' \mid s) = \Pr(S_{t+1} = s' \mid S_t = s)
$$

This means the probability of moving to state $s'$ at time $t+1$ depends only on the current state $s$ at time $t$.

This satisfies the **Markov Property**:

$$
\Pr(S_{t+1} = s' \mid S_t = s, S_{t-1} = s_{t-1}, \dots, S_0 = s_0) = \Pr(S_{t+1} = s' \mid S_t = s)
$$



<h4>Use cases</h4>

Markov Processes are widely used in fields such as:

- **Economics** – Modeling markets and consumer behavior  
- **Biology** – Modeling population or gene transitions  
- **Natural Language Processing (NLP)** – Text generation and tagging  
- **Robotics / AI** – Planning and decision making  
- **Queueing theory** – Modeling customer service or network traffic



  
</div>


<div>
<h3>Introducing Decisions into the Markov Process: MDPs</h3>
  
</div>


