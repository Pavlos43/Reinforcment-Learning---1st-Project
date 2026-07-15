# Reinforcement Learning - 1st Project

Multi-Armed Bandit algorithms applied to wireless channel selection problems using UCB (Upper Confidence Bound) strategy.

## 📋 Project Overview

This project implements and compares two distinct scenarios of the UCB (Upper Confidence Bound) algorithm for solving multi-armed bandit problems in a wireless communication context:

- **Case A**: Joint arm selection with combined feedback
- **Case B**: Per-user independent channel selection

The analysis includes theoretical regret bounds verification and practical performance evaluation through Monte Carlo simulations.

## 🎯 Problem Description

Two users compete for resources across 5 wireless channels with noise-corrupted SNR (Signal-to-Noise Ratio). The goal is to find the optimal channel allocation that maximizes cumulative rewards while minimizing regret.

## 📁 Repository Structure

```
Reinforcment-Learning---1st-Project/
├── README.md                                      # This file
├── Assignment_1.ipynb                            # Main implementation and analysis
└── Reinforcement_Learning_and_Dynamic_Optimization_1.pdf  # Course reference material
```

## 🔧 Key Algorithms & Concepts

### UCB Algorithm (Case A)
- **20 arms**: All possible (user1_channel, user2_channel) combinations where channels differ
- **Strategy**: Joint optimization with single feedback signal
- **Metrics**: Sublinear regret growth, convergence to optimal arm

### UCB Algorithm (Case B)
- **Per-user selection**: User 1 and User 2 independently select channels
- **Constraint**: Users cannot select the same channel simultaneously
- **Strategy**: Separate value estimation with conflict resolution

## 📊 Features

The notebook includes:
- **Theoretical Regret Bounds**: O(log T) complexity verification
- **Practical Regret**: Measured from actual noisy rewards
- **Cumulative Average Reward**: Convergence analysis
- **Arm Selection Distribution**: Visualization of learning patterns
- **Comparative Analysis**: Case A vs Case B performance

## 🚀 Implementation Details

### Parameters
- **K**: 5 wireless channels
- **T_values**: [2000, 20000] time horizons
- **n_mc**: 100 Monte Carlo averages per round
- **SNR Range**: [0.8, 2.0] with noise level ε = 0.6

### Monte Carlo Averaging
Each reward sample is averaged over 100 independent noise realizations to reduce variance in the noisy channel environment.

## 📈 Visualizations

For each algorithm case and time horizon, the following plots are generated:
1. Theoretical vs Practical Regret
2. Cumulative Average Reward Convergence
3. Actual Regret vs O(log t) Theoretical Bound
4. Final Arm Selection Counts

## 📚 Key Results

The implementation validates:
- UCB algorithm achieves sublinear regret growth
- Practical regret closely tracks theoretical predictions
- Optimal arm is identified with high frequency
- Case A and Case B present different trade-offs in convergence

## 📝 Requirements

- Python 3.x
- NumPy
- Matplotlib
- Jupyter Notebook

## 🎓 Course Material

See `Reinforcement_Learning_and_Dynamic_Optimization_1.pdf` for theoretical background on:
- Markov Decision Processes
- Bandit Problems
- UCB Algorithm Theory
- Regret Analysis

## 👤 Author

Pavlos Horn (Pavlos43)

---

For detailed implementation and results, run **Assignment_1.ipynb** in Jupyter Notebook.
