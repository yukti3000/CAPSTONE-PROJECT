# CAPSTONE-PROJECT

📌Autonomous Multi-Agent Collaboration in Dynamic Environments

Hybrid CTDE–Swarm Coordination Simulation (Lightweight Research Implementation)

This repository contains a fully working simulation of a Hybrid Multi-Agent Reinforcement Learning + Swarm Intelligence system, designed to match the research paper:

“Autonomous Multi-Agent Collaboration in Dynamic Environments”

It demonstrates how autonomous agents collaborate, communicate, avoid collisions, and make intelligent decisions in a dynamic & partially observable environment.

⸻

🚀 Project Overview

This project implements a three-layer hybrid architecture, inspired by the research methodology:

✅ 1. Perception Layer
	•	Each agent observes:
	•	Nearby tasks
	•	Nearby agents
	•	Local grid state
	•	Its own energy & capability
	•	Partial observability (limited range using OBS_RANGE).

⸻

✅ 2. Decision Layer

Agents compute a utility score for each visible task:

U = \alpha (-d) + \beta (\text{capability}) + \gamma (\text{priority}) - \delta (\text{energy})

Weights are learned using simple reward-based RL updates.

This layer handles:
	•	Task selection
	•	Energy management
	•	Adaptive re-weighting based on outcomes
	•	Basic decentralized decision-making

⸻

✅ 3. Collaboration Layer

Implements:
	•	Swarm behaviors:
	•	Cohesion (stay with group)
	•	Separation (avoid collisions)
	•	Alignment (follow group direction)
	•	Adaptive communication:
	•	Agents broadcast only when local uncertainty is high
	•	Reduces communication overhead

⸻

🎯 Key Features

✔ Dynamic task spawning
✔ Priority-based task allocation
✔ Swarm intelligence integration
✔ Lightweight RL for utility tuning
✔ Collision detection and avoidance
✔ Adaptive communication mechanism
✔ Real-time visualization
✔ Works in Google Colab with no setup
