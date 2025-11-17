# CAPSTONE-PROJECT

# Autonomous Multi-Agent Collaboration in Dynamic Environments
### *Hybrid CTDE–Swarm Coordination Simulation (Lightweight Research Implementation)*  
### *Capstone Project – Apex Institute of Technology, Chandigarh University*

This repository contains a fully functional simulation of a *Hybrid Multi-Agent Reinforcement Learning (MARL) + Swarm Intelligence architecture*, designed to align with the research paper:

> *“Autonomous Multi-Agent Collaboration in Dynamic Environments”*

The project demonstrates how multiple autonomous agents coordinate, communicate, navigate, avoid collisions, and allocate tasks intelligently in a *dynamic, partially observable grid environment*.

The complete experiment is implemented in *Python* and runs seamlessly in *Google Colab* without external setup.

---

# 🚀 Project Overview

The system implements a *three-layer hybrid architecture*, combining MARL concepts with swarm coordination rules to achieve efficient collaboration among independent autonomous agents.

---

# 🧩 *1. Perception Layer*
Each agent perceives only a *local neighborhood* (partial observability):

- Nearby tasks  
- Nearby agents  
- Grid surroundings  
- Agent capability  
- Agent energy  

This models real-world constraints (e.g., drones, robots, or distributed agents with limited sensors).

---

# 🎛 *2. Decision Layer*

Agents compute a *utility score* for every visible task:

\[
U = \alpha (-d) + \beta (\text{capability}) + \gamma (\text{priority}) - \delta (\text{energy})
\]

Where:
- *d* = distance to task  
- *capability* = heterogeneous skill level of agent  
- *priority* = importance of the task  
- *energy* = agent’s remaining energy  

Agents use *lightweight reinforcement learning* to update these weights based on task success or failure.  
This enables:

- Intelligent task selection  
- Capability-based specialization  
- Energy-aware decision-making  
- Decentralized optimization  

---

# 🤝 *3. Collaboration Layer*

Implements advanced multi-agent cooperation mechanisms:

### 🐝 Swarm Intelligence (Behavioral Rules)
- *Cohesion* → stay near team  
- *Separation* → avoid collisions  
- *Alignment* → move in consistent direction  

These micro-adjustments create realistic distributed movement behavior.

### 📡 Adaptive Communication
Agents broadcast only when needed, based on local uncertainty:
- Reduces communication overhead  
- Emulates decentralized multi-robot systems  
- Prevents unnecessary network load  

---

# 🎯 Key Features

✔ Dynamic environment with continuous task spawning  
✔ Priority-based task assignment  
✔ Hybrid MARL + swarm movement behavior  
✔ Lightweight RL-driven utility tuning  
✔ Collision detection & avoidance  
✔ Communication overhead metrics  
✔ Real-time visualization (Colab-friendly)  
✔ Task decay + lifetime modeling  
✔ Heterogeneous agent capabilities  
✔ Fully reproducible simulation  

---

# 🧪 *Simulation Results (Metrics Tracked)*

The simulation reports:

- *Task Completion Count*  
- *Collision Count*  
- *Communication Overhead*  
- *Agent learning weight updates*  
- *Task density over time*  
- *Agent trajectories*  

These directly correspond to the evaluation metrics in the research paper.

---

# 🖥 *How to Run the Project*

### Option 1: Google Colab (Recommended)
1. Open CAPSTONE_PROJECT.ipynb in Google Colab  
2. Run all cells  
3. Observe:
   - Live multi-agent simulation  
   - Dynamic task updates  
   - Collaboration & swarm behavior  
   - Final results graphs  

No installation required.
