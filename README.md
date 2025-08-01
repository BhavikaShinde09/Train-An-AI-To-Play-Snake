**🐍 Snake AI – Reinforcement Learning with PyTorch & Pygame**


**📌 Overview**

This project implements an AI agent trained to play the classic Snake game using Deep Q-Learning (DQN). Built with PyTorch and Pygame, the agent learns optimal strategies over time by interacting with the environment, receiving rewards, and improving through experience replay.


**🚀 Features**

Full Snake game implemented with Pygame

AI agent using Deep Q-Learning (DQN)

Neural network-based state-action decision making

Reward shaping to encourage learning

Real-time visualization of gameplay


**🗂️ Project Structure**

├── model.py           # Neural network architecture

├── agent.py           # DQN agent logic

├── game.py            # Snake game implementation

├── train.py           # Main training loop


**🛠️ Setup & Installation**

Python 3.8 (e.g. via Anaconda)

PyTorch (CPU or GPU edition)

Pygame, Matplotlib, and other dependencies


**Environment setup**

conda create -n snake-ai python=3.8
conda activate snake-ai


**🤖 How It Works**

**📊 State Representation**

The agent observes the environment through a simplified vector:

Danger ahead, left, right

Direction of movement

Food location relative to head

**🧠 Actions**

The AI can choose from:

Turn Left

Go Straight

Turn Right

**🎯 Reward Function**

+10 for eating food

-10 for dying

0 for every other step

**💡 Learning Mechanism**

Experience replay: past moves stored and sampled

Short and long-term memory training

Q-network updated using Bellman Equation

**📈 Visualization**

After training, the agent's performance is plotted using matplotlib, showing:

Game scores

Average scores per interval
