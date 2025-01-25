# RL Visualizer

RL Visualizer is a Python package for visualizing action probabilities, entropy, and rewards in reinforcement learning models.

## Features

- Visualize action probabilities as bar charts
- Track entropy to monitor model uncertainty
- Plot per-step rewards within a single episode
- Compatible with Gym and Gymnasium environments

## Installation

```bash
pip install rl-visualizer
```
## Example

- Here you can see what rl_visualizer do in action:
- This is a custom highway simulated environment in Gymasium format
- Action space: is defined with this
```python
- Enum class Action(Enum):
    NO_ACTION = 0
    CHANGE_LANE_RIGHT = 1
    CHANGE_LANE_LEFT = 2
    ACCELERATE = 3
    DECELERATE = 4
    EMERGENCY_BRAKE = 5
 ```
 - Given reward for driving between 75km/h and 104km/h (max reward for 104km/h and driving not on leftmost lane)
 - Given extra reward if driving not in the leftmost lane
 - Given negative reward for near collisions and collisions. Near collision is calculated by ttc 
![Image](https://github.com/user-attachments/assets/72280c79-4f85-4391-9f2b-6a1eca5b29dc)
