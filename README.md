# 🐍 Snake AI – Reinforcement Learning with PyTorch & Pygame

## 📌 Overview

This project implements an AI agent trained to play the classic **Snake game** using **Deep Q-Learning (DQN)**. Built with **PyTorch** and **Pygame**, the agent learns optimal strategies over time by interacting with the environment, receiving rewards, and improving through experience replay.

---

## 🚀 Features

- 🎮 Full Snake game implemented with Pygame  
- 🤖 AI agent using Deep Q-Learning (DQN)  
- 🧠 Neural network-based state-action decision making  
- 🏆 Reward shaping to encourage learning  
- 📺 Real-time visualization of gameplay  

---

## 🗂️ Project Structure

```

├── model.py           # Neural network architecture
├── agent.py           # DQN agent logic
├── game.py            # Snake game implementation
├── train.py           # Main training loop

````

---

## 🛠️ Setup & Installation

### ✅ Requirements

- Python 3.8 (recommended via Anaconda)
- PyTorch (CPU or GPU version)
- Pygame
- Matplotlib

### 📦 Environment Setup

```bash
conda create -n snake-ai python=3.8
conda activate snake-ai
pip install -r requirements.txt
````

---

## 🤖 How It Works

### 📊 State Representation

The agent observes the environment using a simplified state vector that includes:

* 🚧 Danger detection (ahead, left, right)
* 🔁 Current movement direction
* 🍎 Relative position of food to the snake's head

### 🧠 Actions

At each step, the agent chooses from:

* 🔄 Turn Left
* ⏩ Go Straight
* 🔁 Turn Right

### 🎯 Reward Function

* ➕ **+10** for eating food
* ❌ **-10** for dying
* ⚪ **0** for a regular move

### 💡 Learning Mechanism

* 🧠 Experience replay: stores and reuses past experiences
* 🕒 Short- and long-term memory training
* 🔁 Q-network updated using the **Bellman Equation**
* 🎲 ε-greedy strategy for balancing exploration and exploitation

---

## 📈 Visualization

After training, a performance graph is plotted using Matplotlib, showing:

* 📊 Game score per episode
* 📉 Average score trend over time

---




