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

## How to Run
Prepare Price Data: Replace the simulated price data in train_trading_agent() with your own time-series data.

Example of simulated data:
np.random.seed(42)

price_data = np.cumsum(np.random.randn(1000)) + 100  # Simulated price data

Train the Model: Run the script to train the agent: python trading_model.py

Output: The script prints the total reward for each training episode, showing how the agent learns over time.

## Customization
Transaction Costs: Adjust the transaction_cost parameter in the TradingEnv class to model real-world trading fees.

State Features: Enhance the state space by adding technical indicators like RSI, MACD, or Bollinger Bands.

Action Space: Modify the action space to include continuous values for fractional trading positions.

Hyperparameters: Tune hyperparameters like learning rate, discount factor, and batch size in the DQNAgent.
