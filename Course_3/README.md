# Prediction and Control with Function Approximation

In this course, you will learn how to solve problems with large, high-dimensional, and potentially infinite state spaces. You will see that estimating value functions can be cast as a supervised learning problem---function approximation---allowing you to build agents that carefully balance generalization and discrimination in order to maximize reward. We will begin this journey by investigating how our policy evaluation or prediction methods like Monte Carlo and TD can be extended to the function approximation setting. You will learn about feature construction techniques for RL, and representation learning via neural networks and backprop. We conclude this course with a deep-dive into policy gradient methods; a way to learn policies directly without learning a value function. In this course you will solve two continuous-state control tasks and investigate the benefits of policy gradient methods in a continuous-action environment. 

Prerequisites: This course strongly builds on the fundamentals of Courses 1 and 2, and learners should have completed these before starting this course.  Learners should also be comfortable with probabilities & expectations, basic linear algebra, basic calculus, Python 3.0 (at least 1 year), and  implementing algorithms from pseudocode.

- By the end of this course, you will be able to: 

  -Understand how to use supervised learning approaches to approximate value functions;
  -Understand objectives for prediction (value estimation) under function approximation;
  -Implement TD with function approximation (state aggregation), on an environment with an infinite state space (continuous state space);
  -Understand fixed basis and neural network approaches to feature construction;
  -Implement TD with neural network function approximation in a continuous state environment;
  -Understand new difficulties in exploration when moving to function approximation;
  -Contrast discounted problem formulations for control versus an average reward problem formulation;
  -Implement expected Sarsa and Q-learning with function approximation on a continuous state control task;
  -Understand objectives for directly estimating policies (policy gradient objectives);
  -Implement a policy gradient method (called Actor-Critic) on a discrete state environment.
  
  ## On-policy Prediction with Approximation
  
  In this module, you will learn how to estimate a value function for a given policy, when the number of states is much larger than the memory available to the agent. You will learn how to specify a parametric form of the value function, how to specify an objective function, and how estimating gradient descent can be used to estimate values from interaction with the world.
  
  ## Constructing Features for Prediction
  
  The features used to construct the agent’s value estimates are perhaps the most crucial part of a successful learning system. In this module we discuss two basic strategies for constructing features: (1) fixed basis that form an exhaustive partition of the input, and (2) adapting the features while the agent interacts with the world via Neural Networks and Backpropagation. In this week’s graded assessment you will solve a simple but infinite state prediction task with a Neural Network and TD learning.
  
  ## Control with Approximation
  
  Now, you will see that the concepts and tools introduced in modules two and three allow straightforward extension of classic TD control methods to the function approximation setting. In particular, you will learn how to find the optimal policy in infinite-state MDPs by simply combining semi-gradient TD methods with generalized policy iteration, yielding classic control methods like Q-learning, and Sarsa. We conclude with a discussion of a new problem formulation for RL---average reward---which will undoubtedly be used in many applications of RL in the future.
  
  ## Policy Gradient
  
  Every algorithm you have learned about so far estimates a value function as an intermediate step towards the goal of finding an optimal policy. An alternative strategy is to directly learn the parameters of the policy. This week you will learn about these policy gradient methods, and their advantages over value-function based methods. You will also learn how policy gradient methods can be used to find the optimal policy in tasks with both continuous state and action spaces.
