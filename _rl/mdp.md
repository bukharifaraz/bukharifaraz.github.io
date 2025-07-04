---
layout: single
title:  "Markov Decision Process (MDP)"
classes: wide
date:   2025-07-04 13:32:01 +0530
categories: RL ML AI
tags: RL
---

<div>
<h3>Markov Process</h3>

A \textbf{Markov Process} is a type of stochastic (random) process that satisfies the \textit{Markov property} — the principle that the future state of a system depends only on the present state, not on the sequence of events that preceded it.

\section*{Layman Definition}

In simple terms, a Markov Process is like a memoryless system: where you are now is all that matters in determining where you go next. The path you took to get here doesn’t affect your next step.

\section*{Formal Definition}

A Markov Process is formally defined as a tuple:
\[
(S, P)
\]
where:

\begin{itemize}[leftmargin=2em]
    \item $S$ is a (finite or infinite) set of states.
    \item $P$ is a transition probability matrix or function, where:
    \[
    P(s' \mid s) = \Pr(S_{t+1} = s' \mid S_t = s)
    \]
    This means that the probability of moving to state $s'$ at time $t+1$ depends only on the current state $s$ at time $t$.
\end{itemize}

This satisfies the \textbf{Markov Property}:
\[
\Pr(S_{t+1} = s' \mid S_t = s, S_{t-1} = s_{t-1}, \dots, S_0 = s_0) = \Pr(S_{t+1} = s' \mid S_t = s)
\]

\section*{Use Cases of Markov Processes}

Markov Processes are widely used in various domains, including:

\begin{itemize}[leftmargin=2em]
    \item \textbf{Economics}: Modeling market trends and consumer behavior.
    \item \textbf{Biology}: Modeling gene expression and evolutionary dynamics.
    \item \textbf{Natural Language Processing (NLP)}: Markov models for text generation.
    \item \textbf{Robotics and AI}: Planning and reinforcement learning.
    \item \textbf{Queueing theory}: Analyzing systems with random service and arrival times.
\end{itemize}


  
</div>


<div>
<h3>Introducing Decisions into the Markov Process: MDPs</h3>
  
</div>


