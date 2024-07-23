# Reinforcement Learning Projects

This repository contains the code and reports for two major projects completed as part of the Reinforcement Learning course at Reichman University. The projects explore classical tabular reinforcement learning methods and deep reinforcement learning techniques applied to MiniGrid environments.

## Table of Contents
- [Introduction](#introduction)
- [Projects Overview](#projects-overview)
  - [MidProject: Classical Tabular Reinforcement Learning](#midproject-classical-tabular-reinforcement-learning)
  - [FinalProject: Deep Reinforcement Learning](#finalproject-deep-reinforcement-learning)
- [Acknowledgments](#acknowledgments)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This repository documents my journey in solving two variations of the MiniGrid environment, initially using classical tabular reinforcement learning methods and subsequently transitioning to deep reinforcement learning techniques. The MiniGrid environment provides a lightweight, 2D grid-world setting with goal-oriented tasks, challenging the agent to solve different maze maps and interact with various objects.

## Projects Overview

### MidProject: Classical Tabular Reinforcement Learning

**Report:** [REPORT_MidProject.pdf](./REPORT_MidProject.pdf)  
**Notebook:** [RL2024_MidProject.ipynb](./RL2024_MidProject.ipynb)

In this project, I implemented classical reinforcement learning algorithms from scratch, including Monte Carlo, SARSA, and Q-Learning. These algorithms were applied to two distinct MiniGrid environments:

1. **RandomEmptyEnv_10:** The agent navigates a maze to reach a designated goal. This environment tests the agent's learning and adaptation capabilities in a relatively simpler setting.
2. **RandomKeyMEnv_10:** The agent must find a key, unlock a door, and then reach the goal. This environment presents a higher level of complexity, requiring sequential decision-making and interaction with objects.

**Key Features:**
- **State Representation:** The environment states were encoded into hashable tuples for efficient Q-table management. This ensured unique state identification and fast lookups.
- **Reward Shaping:** Custom reward structures were designed to guide the agent's learning process effectively. This included rewards for reaching goals and penalties for inefficient actions.
- **Hyperparameter Tuning:** Extensive tuning of gamma (discount factor), alpha (learning rate), and epsilon (exploration rate) parameters to optimize learning performance. The choice of hyperparameters significantly influenced the learning dynamics and efficiency.

### FinalProject: Deep Reinforcement Learning

**Report:** [REPORT_FinalProject.pdf](./REPORT_FinalProject.pdf)  
**Notebook:** [RL2024_FinalProject.ipynb](./RL2024_FinalProject.ipynb)

The final project focused on implementing and comparing advanced deep reinforcement learning algorithms in the same MiniGrid environments. I developed the following deep RL algorithms from scratch:

1. **Standard DQN:** Utilizes a simple Q-network to estimate the action-value function.
2. **Double DQN:** Addresses overestimation bias by decoupling the selection and evaluation of actions.
3. **Dueling DQN:** Introduces separate estimations of state values and action advantages, facilitating more efficient learning.
4. **Dueling Double DQN:** Combines the advantages of Double DQN and Dueling DQN for enhanced performance.

**Key Features:**
- **Preprocessing:** Included steps such as edge cropping, grayscale conversion, normalization, and resizing of pixel-based observations to facilitate efficient neural network training.
- **Reward Shaping:** Refined reward structures to incentivize efficient task completion, including step penalties and rewards for key interactions.
- **Replay Buffer:** Implemented to store and replay past experiences, breaking the correlation between consecutive samples and stabilizing learning.
- **Q-Networks:** Designed convolutional neural networks (CNNs) to estimate Q-values from preprocessed state images. The network architecture included convolutional and fully connected layers to extract features and map them to action values.

## Acknowledgments

This repository and the projects it contains were developed as part of the Reinforcement Learning course at Reichman University. I would like to extend my gratitude to my professor, [Professor's Name], for their invaluable guidance and support throughout the course.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or suggestions.

