# Echo Chamber Simulation

An agent-based simulation of echo chamber dynamics using the Voter Model.

## Overview

This project reproduces the findings of my undergraduate thesis (Tohoku University, 2021), which investigated how cross-group connections affect opinion convergence in polarized networks.

**Research Question:** When agents with cross-group bridges and agents without them coexist, does the ratio of bridge-holding agents affect overall opinion convergence?

**Key Findings:**
- Convergence rate increases non-linearly with the number of bridges. Even a small proportion (20–30%) of bridge-holding nodes significantly raises the probability of network-wide consensus.
- While bridges increase the probability of convergence, they do not affect the time it takes to converge. Average convergence time remains stable regardless of the number of bridges.

## Model

- Based on the **Voter Model** (Holley & Liggett, 1975)
- Two fully-connected groups of N nodes each (2N total)
- Bridge edges connect nodes across groups
- Opinion values: 0 or 1 (binary)

## Simulations

### 1. Opinion Convergence Process
Visualizes how opinions evolve over time, comparing networks with and without bridges.

### 2. Convergence Rate by Bridge Count
Runs 100 trials per bridge count to measure how the proportion of bridge-holding nodes affects the probability of network-wide consensus.

### 3. Convergence Rate by Network Size
Replicates the above analysis across four network sizes (Node=10, 30, 50, 100) to verify the pattern holds regardless of scale.

### 4. Average Convergence Time by Network Size
Measures the average number of time steps needed to reach consensus, showing that bridge count does not significantly affect convergence speed.

## Tech Stack

- Python
- NetworkX
- NumPy
- Matplotlib
- Google Colab

## How to Run

Open the notebook in Google Colab and run all cells in order.
