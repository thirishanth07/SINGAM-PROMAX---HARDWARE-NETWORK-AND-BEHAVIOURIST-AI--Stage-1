# Chapter 7: Introduction to Behaviorist AI

**AI focused on observable actions and how experience shapes them.**

## Learning Objectives

By the end of this chapter, readers should be able to:

- Define Behaviorist AI and its main principles.
- Compare behaviorism and cognitivism.
- Identify agents, environments, observations, and actions.
- Explain the agent-environment loop.
- Describe how AI agents perceive, decide, and act.

## Behaviorism vs. Cognitivism

| Perspective | Definition / Focus | Maze Example |
|---|---|---|
| **Behaviorism** | Observable behaviour: actions that can be seen or measured, and how experience shapes them. | How does feedback change the robot's actions? |
| **Cognitivism** | Internal processes such as memory, reasoning, and planning. | How does the robot use a remembered map? |

*Note: These are two perspectives on intelligence; they can overlap in AI systems.*

## What is an AI Agent?

An agent observes its environment and chooses actions to achieve a goal.

| Term | Definition | Maze Example |
|---|---|---|
| **Agent** | Decision-making system. | The robot. |
| **Environment** | Surroundings it interacts with. | The maze. |
| **Observation** | Sensor information received. | Nearby walls. |
| **Action** | Operation the agent performs. | Move forward or turn. |
| **Goal** | Intended result. | Reach the exit. |

*An agent may use programmed rules or a learned strategy.*

## The Agent-Environment Loop

1. **Observe:** Detect nearby walls.
2. **Choose:** Select a turn.
3. **Act:** Motors turn the robot.
4. **Observe Again:** Receive new sensor information.

*During reinforcement learning, the agent also receives numerical rewards.*

## Perception, Decision & Action

| Step | Definition | Maze Example |
|---|---|---|
| **Perception** | Interpreting sensor information. (What is around me?) | Sensors detect a wall ahead. |
| **Decision** | Choosing what to do. (What should I do?) | The policy chooses a left turn. |
| **Action** | An operation affecting the environment. (Carry it out) | Motors turn the robot left. |

**Policy** = strategy for choosing actions. Detecting, choosing, and acting are separate steps.

## Chapter Summary

- Behaviorist AI focuses on observable actions and learning from experience.
- Behaviorism studies actions, while cognitivism focuses on internal thinking processes.
- AI agents observe their environment and take actions to achieve goals.
- The agent-environment loop is a continuous cycle of observing and acting.
- AI agents use perception, decision-making, and action to interact with their surroundings.
