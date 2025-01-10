# Deep Q-Learning Trading Model

This project implements a simplified Deep Q-Learning model for trading financial assets. It uses reinforcement learning to train an agent that directly interacts with a simulated trading environment to optimize trading strategies.

## Features

- **Deep Q-Learning**: Implements a Q-network to estimate state-action values for trading decisions.
- **Trading Environment**: Simulates a financial market with discrete actions: short, neutral, and long positions.
- **Transaction Costs**: Incorporates transaction costs to make the model more realistic.
- **Experience Replay**: Uses a replay buffer to stabilize training.
- **Target Network**: Includes a target Q-network for better training stability.

## Requirements

To run the project, you need Python 3.7+ and the following libraries:

- `numpy`
- `pandas`
- `torch`

