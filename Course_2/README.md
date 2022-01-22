# Sample-based Learning Methods

In this course, you will learn about several algorithms that can learn near optimal policies based on trial and error interaction with the environment---learning from the agent’s own experience. Learning from actual experience is striking because it requires no prior knowledge of the environment’s dynamics, yet can still attain optimal behavior. We will cover intuitively simple but powerful Monte Carlo methods, and temporal difference learning methods including Q-learning. We will wrap up this course investigating how we can get the best of both worlds: algorithms that can combine model-based planning (similar to dynamic programming) and temporal difference updates to radically accelerate learning.

- By the end of this course you will be able to:
 
  - Understand Temporal-Difference learning and Monte Carlo as two strategies for estimating value functions from sampled experience;
  - Understand the importance of exploration, when using sampled experience rather than dynamic programming sweeps within a model;
  - Understand the connections between Monte Carlo and Dynamic Programming and TD;
  - Implement and apply the TD algorithm, for estimating value functions;
  - Implement and apply Expected Sarsa and Q-learning (two TD methods for control); 
  - Understand the difference between on-policy and off-policy control;
  - Understand planning with simulated experience (as opposed to classic planning strategies);
  - Implement a model-based approach to RL, called Dyna, which uses simulated experienc;
  - Conduct an empirical study to see the improvements in sample efficiency when using Dyna.

## Monte Carlo Methods for Prediction & Control

How to estimate value functions and optimal policies, using only sampled experience from the environment. This module represents our first step toward incremental learning methods that learn from the agent’s own interaction with the world, rather than a model of the world. You will learn about on-policy and off-policy methods for prediction and control, using Monte Carlo methods---methods that use sampled returns. You will also be reintroduced to the exploration problem, but more generally in RL, beyond bandits.

## Temporal Difference Learning Methods for Prediction

In this module you will learn about one of the most fundamental concepts in reinforcement learning: temporal difference (TD) learning. TD learning combines some of the features of both Monte Carlo and Dynamic Programming (DP) methods. TD methods are similar to Monte Carlo methods in that they can learn from the agent’s interaction with the world, and do not require knowledge of the model. TD methods are similar to DP methods in that they bootstrap, and thus can learn online---no waiting until the end of an episode. You will see how TD can learn more efficiently than Monte Carlo, due to bootstrapping. For this module, we first focus on TD for prediction, and discuss TD for control in the next module. On this module, you will implement TD to estimate the value function for a fixed policy, in a simulated domain.

## Temporal Difference Learning Methods for Control

Now, you will learn about using temporal difference learning for control, as a generalized policy iteration strategy. You will see three different algorithms based on bootstrapping and Bellman equations for control: Sarsa, Q-learning and Expected Sarsa. You will see some of the differences between the methods for on-policy and off-policy control, and that Expected Sarsa is a unified algorithm for both. You will implement Expected Sarsa and Q-learning, on Cliff World.

## Planning, Learning & Acting

Up until now, you might think that learning with and without a model are two distinct, and in some ways, competing strategies: planning with Dynamic Programming verses sample-based learning via TD methods. This week we unify these two strategies with the Dyna architecture. You will learn how to estimate the model from data and then use this model to generate hypothetical experience (a bit like dreaming) to dramatically improve sample efficiency compared to sample-based methods like Q-learning. In addition, you will learn how to design learning systems that are robust to inaccurate models.
