# Reinforcement Learning (RL) Benchmark

This folder presents an example of how to use QlibRL to run a reinforcement learning job. In this example, we will show you how to launch an RL task through configuration files on the built-in order execution scene of Qlib.

## Scenario

This example is based on the built-in **order execution** scenario of Qlib. Order execution is a fundamental problem in algorithmic trading that aims at fulfilling a specific trading order, either liquidation or acquirement, for a given instrument. For more details about the scenario, please refer to this [doc](https://qlib.readthedocs.io/en/latest/component/rl/overall.html#order-execution). As a reference, the logic of the built-in order execution scenario is implemented in `qlib/rl/order_execution/simulator_simple.py`.

## Data Processing

For Feature processing, we take Yahoo dataset as an example.

To get data, run (this takes 10~20 minutes):

``python data_process.py``

For order generation, run:

``python order_gen.py``

The generated data will be stored in `data/`.

## Training and Backtest


