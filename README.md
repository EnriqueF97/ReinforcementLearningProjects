# Reinforcement Learning with OpenAI Gym: Taxi and LunarLander

This repository demonstrates classic and deep reinforcement learning algorithms applied to two standard OpenAI Gym environments: Taxi-v3 and LunarLander-v3.

## Overview

- **Taxi-v3:**  
  A simple, fully discrete environment used to demonstrate Tabular Q-learning.

- **LunarLander-v3:**  
  A continuous, high-dimensional environment used to demonstrate:
  - Tabular Q-learning (with state discretization)
  - Deep Q-Network (DQN)
  - Double Deep Q-Network (Double DQN)

## Algorithms

### Tabular Q-learning

Tabular Q-learning is implemented for both Taxi and discretized LunarLander.

- For Taxi-v3, the small and finite state space allows exact representation of the Q-values.
- For LunarLander-v3, the continuous state space is discretized into bins to allow tabular learning, but performance is limited compared to function approximation methods.

### Deep Q-Network (DQN)

DQN uses a neural network to approximate the Q-function, enabling the agent to generalize across the vast, continuous state space of LunarLander. The DQN implementation includes:

- Experience replay buffer
- Target network for stable updates
- Epsilon-greedy exploration

### Double DQN

Double DQN further improves stability and learning by decoupling action selection and evaluation when computing the target Q-values, reducing the overestimation bias inherent in standard DQN.

## Requirements

- Python 3.8+
- `gymnasium`
- `numpy`
- `matplotlib`
- `torch`
- `tqdm`

To install the requirements execute these colab files in a new colab project (Clean and OS independant), or install them directly by executing the files (Not recommended for environment libraries clash).
