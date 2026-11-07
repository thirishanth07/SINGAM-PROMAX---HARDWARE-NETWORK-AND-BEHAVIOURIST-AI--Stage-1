# Chapter 10: Applications of Behaviorist AI

## Learning Objectives

**Main Goal:** Explore how Behaviorist AI is used in robotics, games, and practical systems that respond to experience.

By the end of this chapter, you should be able to:

- Describe how Behaviorist AI is used in robotics and games.
- Explain how rewards and feedback influence game agents.
- Identify uses in smart homes, healthcare, and driving.
- Describe how robots improve actions through experience.
- Distinguish learned behaviour from fixed-rule responses.

## Real-World Applications

**Simulation** = a computer-made environment for training or testing.

| Task | Possible Approach | Learning Signal |
|---|---|---|
| Playing a game | Reinforcement learning | Scores or win/loss rewards |
| Learning robotic movement | RL, often in simulation | Rewards for task performance |
| Picking up an object | Behavioral cloning | Human operator demonstrations |

*Note: The task alone does not tell us which learning method was used.*

## From Feedback to Learned Behaviour

The core loop is: **OBSERVE → ACT → RECEIVE FEEDBACK → LEARN**

| Application | Example of Learned Behaviour |
|---|---|
| **Smart Home** | Adjust lighting based on resident feedback. |
| **Care Support** | Learn support tasks from caregiver demonstrations. |
| **Robot** | Practise actions and use success to improve. |
| **Driving** | Learn driving actions from expert examples. |

*Note: Fixed-rule automation is not automatically behaviorist AI; learning needs feedback or demonstrations.*

## Robotics & Learning-Based Driving

- **Robotics:** A robot learns gesture responses from examples.
- **Driving Assistance:** A driving policy can learn from expert examples.

*Note: These are learning-based possibilities, not features of every system. Driving requires safety validation.*

### Robotics: Learning Through Action

**How a Robot Learns:**
1. **Observe:** Sensors detect objects, distances, and robot position.
2. **Act:** The robot moves, turns, or controls a gripper.
3. **Improve:** Feedback or demonstrations help refine future actions.

**Example: Picking up an Object**
1. Detect the object and estimate its position.
2. Choose an arm movement and grip.
3. Attempt to pick up the object.
4. Use success or failure to improve.

## Game-Playing Agents

Game-playing agents learn through repeated interaction with a simulated world.

| Element | Definition | Example |
|---|---|---|
| **Agent** | An AI player that chooses actions. | Move, jump, or turn. |
| **Environment** | The game world and its rules. | Maze, opponents, or obstacles. |
| **Reward** | Feedback on the result of an action. | Score, victory, or a penalty. |

*The agent learns to select actions that can increase its long-term reward.*

**The Learning Loop:**
1. **Try:** Choose a direction in the maze.
2. **Receive Feedback:** Get a reward or a penalty.
3. **Update:** Improve the action strategy.
4. **Repeat:** Try again and find a better route.

*Example rewards: exit +20 | hit wall -5 | step -1. Rewards are illustrative; the objective is to learn a successful strategy.*

## Adaptive Smart Home

Adaptive lighting improves using repeated feedback.

- **Observe:** Occupancy and residents' preferences.
- **Act:** Adjust lighting or temperature.
- **Feedback:** Resident changes an unwanted setting.
- **Learn:** Improve choices for similar situations.

## Healthcare: Learning Assistive Tasks

Wearables can inform assisted activity. An assistive robot can learn tasks through demonstration.

1. **Demonstrate:** Caregiver shows a safe movement.
2. **Practise:** Robot attempts a suitable assistance task.
3. **Feedback:** Success and corrections guide learning.
4. **Improve:** Robot refines its next action.

## Chapter Summary

- Robots can learn navigation, movement, and object handling through feedback.
- Game agents learn by trying actions and receiving rewards or penalties.
- Adaptive smart homes and assistive robots can improve through feedback.
- Learning-based robotics and driving policies may use expert demonstrations.
- Fixed-rule responses alone are not learning; testing and oversight remain essential.
