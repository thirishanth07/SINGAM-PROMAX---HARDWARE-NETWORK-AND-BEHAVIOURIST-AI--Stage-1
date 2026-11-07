# Chapter 8: Fundamentals of Reinforcement Learning

## Learning Objectives

By the end of this chapter, readers should be able to:

- Define reinforcement learning and explain how it works.
- Identify the key components of reinforcement learning.
- Explain how rewards and penalties influence learning.
- Understand Markov Decision Processes (MDPs).
- Describe how states, actions, and rewards are connected.

## Reinforcement Learning (RL)

Reinforcement learning (RL) is learning actions that increase total reward over time.

- **Training** = adjusting the policy using experience.

**How it Works:**
1. Try a route through the maze.
2. Receive rewards based on the outcome.
3. Training updates the action strategy.
4. Repeat over many attempts.

**Policy** = the agent's strategy for choosing actions.

## Rewards and Penalties

- **Reward:** Numerical feedback used during learning.
- **Penalty:** Negative reward.
- **Total reward:** Sum of rewards across steps.

| Outcome | Example Reward | Purpose |
|---|---|---|
| Reach the exit | +20 | Encourage completing the task. |
| Hit a wall | -5 | Discourage collisions. |
| Take an ordinary step | -1 | Encourage shorter routes. |

*Illustrative values. The aim is a higher TOTAL reward across the journey.*

## Key Components of Reinforcement Learning

| Term | Definition |
|---|---|
| **Agent** | The AI system that makes decisions and learns. |
| **Environment** | The world in which the agent operates. |
| **State** | The current situation of the environment. |
| **Action** | A decision or movement made by the agent. |
| **Reward** | Numerical feedback received after an action. |

## Markov Decision Process (MDP)

A Markov Decision Process is a mathematical framework used to model decision-making in situations where actions influence future outcomes.

| Component | Definition |
|---|---|
| **States (S)** | Possible situations the agent can be in. |
| **Actions (A)** | Choices available to the agent. |
| **Transition (P)** | Probability of moving from one state to another. |
| **Rewards (R)** | Feedback received after taking an action. |

## Chapter Summary

- Reinforcement learning allows AI agents to learn through trial and error.
- Agents receive rewards and penalties based on their actions.
- The goal is to maximize cumulative rewards over time.
- States, actions, and rewards are essential components of reinforcement learning.
- Markov Decision Processes provide a framework for understanding sequential decision-making.
