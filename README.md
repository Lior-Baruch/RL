# Reinforcement Learning in MiniGrid Environments

## Overview

This project delves into the application and optimization of reinforcement learning (RL) algorithms within the MiniGrid environment, focusing on two distinct challenges: the `Empty Environment` and the `Key Environment`. Through rigorous experimentation with Monte Carlo, SARSA, and Q-Learning algorithms, we aim to uncover effective strategies for agent navigation and task completion, emphasizing the importance of hyperparameter tuning in achieving optimal algorithmic performance.

## Environment Setup

Our study utilizes the `gym-minigrid` package to create a simplified gridworld setting that serves as a versatile platform for testing RL algorithms. This setup allows us to simulate a range of tasks, from basic navigation to complex scenarios involving object interactions, under controlled conditions. The environments are specifically chosen to test both the agent's basic movement capabilities and its ability to perform more sophisticated operations, such as key retrieval and door unlocking.

## Algorithmic Approach

### Monte Carlo Control
This algorithm estimates action-value functions based on episodic sampling, with policies derived from these estimations. It’s particularly useful for environments where the model dynamics are unknown, relying on experience to inform policy improvement.

### SARSA (State-Action-Reward-State-Action)
An on-policy temporal difference learning method, SARSA updates value estimates based on the current policy's observed transitions. This approach directly incorporates the policy's exploration strategy into its value estimation, making it adept at learning policies that balance the exploration-exploitation trade-off.

### Q-Learning
An off-policy learner, Q-Learning seeks the optimal action-value function, regardless of the policy followed by the agent. This method's strength lies in its ability to evaluate the potential of actions independently, promoting efficient policy optimization.

## Hyperparameter Optimization

A systematic grid search was employed to fine-tune hyperparameters such as the exploration rate (epsilon), discount factor (gamma), and learning rate (alpha). This process is crucial for identifying configurations that maximize the agent's performance in terms of reward accumulation and goal achievement efficiency.

## Evaluation and Insights

Post-training, we conducted a detailed evaluation of the generated policies, assessing their effectiveness based on average rewards, steps to goal, and success rates. The project also offers visual demonstrations of the agent's behavior under optimal policies, providing intuitive insights into the strategies learned by the agent.

## Project Structure

The project is organized as follows:

1. **Environment Initialization**: Scripts and instructions for setting up the MiniGrid environments.
2. **Algorithm Implementation**: Code modules for each RL algorithm, designed with adaptability and efficiency in mind.
3. **Hyperparameter Tuning**: Scripts for conducting the grid search, including parameter range definitions and evaluation metrics.
4. **Evaluation**: Tools for assessing algorithm performance, featuring reward and step history visualization.
5. **Inference and Visualization**: Functions for demonstrating the agent's behavior in the environment, highlighting the practical applications of the learned policies.

## Getting Started

To replicate our study or extend it with your own experiments, follow these steps:

1. **Install Dependencies**: Ensure all required packages are installed according to the provided setup instructions.
2. **Initialize Environments**: Use the environment setup scripts to prepare the MiniGrid scenarios.
3. **Train Agents**: Execute the algorithm-specific scripts to start the training process, exploring different hyperparameter settings.
4. **Optimize Hyperparameters**: Apply the grid search scripts to identify the best hyperparameter configurations.
5. **Evaluate Policies**: Assess the performance of the derived policies using the evaluation tools.
6. **Visualize Performance**: Explore the agent's decision-making process in the MiniGrid environments through the provided visualization scripts.

## Conclusion

This project underscores the critical role of algorithm selection, hyperparameter optimization, and strategic reward shaping in solving complex RL tasks. Our findings highlight Q-Learning's adaptability and robustness across varied scenarios, offering valuable insights for future research and applications in reinforcement learning.
