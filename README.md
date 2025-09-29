# Q-Learning in the Frozen Lake Environment

This repository contains the implementation and analysis of the **Q-Learning algorithm** applied to the Frozen Lake environment using the Gymnasium library. The work was conducted as part of the *Neuroscience of Learning, Cognition and Memory* course project at Sharif University of Technology.

---

## Project Overview

The objective of this project is to train an agent to navigate the Frozen Lake environment efficiently by learning an optimal policy through reinforcement learning. The environment simulates uncertainty in navigation, requiring the agent to reach a goal while avoiding holes. Both deterministic (non-slippery) and stochastic (slippery) modes were studied to evaluate learning stability and adaptability.

Key aspects of the project include:

- Implementation of **Q-Learning** with a tabular Q-Table approach.  
- Hyperparameter tuning, including learning rate, discount factor, and exploration rate with decay.  
- Comparison of deterministic and stochastic environments to assess the impact of uncertainty.  
- **Reward shaping** experiments, introducing movement penalties and goal bonuses to accelerate convergence.  
- **Parameter sweep analysis**, exploring the effects of fixed vs. decaying learning and exploration rates.  
- **Visualization and video recording** of agent behavior and policies during training and evaluation.  

---

## Repository Structure

- `notebooks/`: Code implementing Q-Learning training, evaluation, and visualization.  
- `videos/`: Recorded videos of training progression and greedy policy executions.  
- `Report.pdf`: Full project report with methodology, results, and analysis.  
- `.gitignore`: Ignore rules for local files.  

---

## Results Summary

- In deterministic environments, the agent converged rapidly to an optimal policy, consistently reaching the goal in six steps.  
- In stochastic environments, training required significantly more episodes and resulted in less stable performance, highlighting the challenge of uncertainty.  
- Reward shaping accelerated learning without sacrificing policy quality, with goal bonuses producing the fastest convergence.  
- Decaying exploration strategies (epsilon decay) improved stability and convergence speed compared to fixed exploration rates.  
- Visualizations confirmed that the agent transitioned from random exploration to efficient, goal-directed navigation.  
