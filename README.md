# Reinforcement Learning - 1st Project

A comprehensive reinforcement learning project exploring fundamental RL concepts and algorithms.

## 📋 Overview

This project implements core reinforcement learning algorithms and concepts, providing hands-on experience with:
- Markov Decision Processes (MDPs)
- Value iteration and policy iteration
- Q-learning and temporal difference learning
- Environment interaction and agent training

## 🚀 Getting Started

### Prerequisites

- Python 3.7+
- NumPy
- Matplotlib (for visualization)
- OpenAI Gym (for environments)

### Installation

```bash
git clone https://github.com/Pavlos43/Reinforcment-Learning---1st-Project.git
cd Reinforcment-Learning---1st-Project
pip install -r requirements.txt
```

## 📁 Project Structure

```
├── README.md
├── requirements.txt
├── algorithms/
│   ├── value_iteration.py
│   ├── policy_iteration.py
│   └── q_learning.py
├── environments/
│   └── custom_env.py
└── main.py
```

## 🔧 Algorithms Implemented

### 1. Value Iteration
Dynamic programming algorithm for finding optimal value functions.

### 2. Policy Iteration
Iterative algorithm that alternates between policy evaluation and improvement.

### 3. Q-Learning
Model-free temporal difference algorithm for off-policy learning.

## 📊 Results & Visualization

Results and training curves are saved in the `results/` directory with visualizations of:
- Cumulative rewards over episodes
- Learning progress
- Policy convergence

## 💡 Usage

Run the main script to execute the RL algorithms:

```bash
python main.py
```

## 📚 References

- Sutton & Barto: Reinforcement Learning (2nd Edition)
- OpenAI Gym Documentation
- Deep RL Course Materials

## 📝 License

This project is for educational purposes.

## 👤 Author

Pavlos43

---

For questions or improvements, feel free to open an issue or submit a pull request!
