# Chapter 9: Reinforcement Learning Algorithms

## Learning Objectives

By the end of this chapter, readers should be able to:

- Explain the purpose of reinforcement learning algorithms.
- Describe how Q-Learning and Deep Q-Networks work.
- Understand policy gradient methods.
- Explain exploration and exploitation.
- Compare reinforcement learning with behavioral cloning.

## Introduction to RL Algorithms

A reinforcement learning algorithm helps an AI agent learn which actions to take by interacting with its environment and receiving rewards.

**How it Works:**
1. **Observe:** The agent receives information about its current situation.
2. **Act:** The agent chooses an action and receives feedback.
3. **Learn:** The algorithm updates its strategy to improve future decisions.

**Example:** A robot explores a maze, learns from rewards and penalties, and gradually discovers a better route to the exit.

## Q-Learning

Q-Learning helps an agent learn the value of taking different actions in different situations. A **Q-value** estimates the future rewards of taking an action in a state.

**How it Works:**
1. **Observe:** Identify the current state.
2. **Choose:** Select an action.
3. **Get a Reward:** Receive feedback from the environment.
4. **Update:** Revise the action's Q-value.
5. **Repeat:** Keep learning through experience.

**Example:** A robot learns which direction to move in a maze. Actions that lead to better rewards get higher Q-values.

## Deep Q-Network (DQN)

A Deep Q-Network uses a neural network to estimate Q-values for different actions. This helps when there are too many possible states for a simple Q-table.

**How it Works:**
1. **Input:** Feed information about the current state into the network.
2. **Estimate:** Predict Q-values for the available actions.
3. **Select:** Choose an action using those values, sometimes exploring.
4. **Learn:** Train the network on experiences and rewards.

**Example:** A video game agent uses screen images to estimate which button press may lead to better rewards.

## Policy Gradient Methods

A **policy** is a strategy for choosing actions. Policy gradient methods adjust that strategy directly to increase expected rewards.

**How it Works:**
1. **Choose an Action:** Use the current policy to select an action.
2. **Get Feedback:** Interact with the environment and receive rewards.
3. **Improve the Policy:** Make rewarding actions more likely in similar situations.

**Example:** A robot learns to balance by adjusting the probabilities of different movements based on experience.

## Exploration vs. Exploitation

An agent balances trying new actions with using actions that already appear successful.

- **Exploration:** Try new actions to discover potentially better rewards. (e.g., A robot tries a new route through a maze to see if it reaches the exit faster.)
- **Exploitation:** Choose actions that already appear to give good results. (e.g., A robot follows a route that has worked before.)

*Too much exploration can waste time on poor actions. Too much exploitation can hide better strategies. A balance helps the agent learn while earning rewards.*

## Behavioral Cloning (BC)

Behavioral cloning means learning a policy from expert demonstrations.

- A **policy model** is a learned system that selects an action from an observation.

**How it Works:**
1. **Demonstrate:** A skilled demonstrator controls the robot through the maze.
2. **Record:** Save each observation with the expert's action.
3. **Train:** Learn to predict the expert's action from an observation.
4. **Use:** Choose actions in similar situations.

## RL vs. Behavioral Cloning

**Training signal** = information used to adjust a model during learning.

| Feature | Reinforcement Learning | Behavioral Cloning |
|---|---|---|
| **Training Signal** | Numerical rewards. | Expert example actions. |
| **Training Goal** | Increase total reward. | Predict demonstrated actions. |
| **Maze Example** | Practise routes and learn from rewards. | Learn from expert-controlled journeys. |
| **Challenge** | Many attempts; careful reward design. | Unfamiliar situations missing from examples. |

*RL learns from rewards. BC learns from demonstrated actions. They can be combined.*

## Comparison of RL Algorithms

| Feature | Q-Learning | DQN | Policy Gradient |
|---|---|---|---|
| **Main Approach** | Learns action values. | Uses a neural network to estimate Q-values. | Learns a policy directly. |
| **Learning Method** | Updates a Q-table in basic tabular form. | Trains a neural network. | Adjusts policy parameters. |
| **Suitable For** | Small, discrete state-action spaces. | Large or complex state spaces with discrete actions. | Discrete or continuous action spaces, depending on method. |
| **Example** | Solving a simple maze. | Playing video games using screen images. | Controlling robot movements. |

## Chapter Summary

- RL algorithms help agents improve their decisions through experience.
- Q-Learning learns action values to guide decisions.
- Deep Q-Networks use neural networks to estimate action values.
- Policy gradient methods directly improve an agent's policy.
- Exploration and exploitation must be balanced during learning.
- Behavioral cloning learns from expert demonstrations rather than rewards.
