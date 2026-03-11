<img width="2816" height="1536" alt="intro" src="https://github.com/user-attachments/assets/3ed785fb-900a-4b49-85f5-484b0a71af20" />

OPEN QUANTUM SYSTEMS

QUANTUM COLLISION MODELS

NON-MARKOV AND MARKOV APPROACHES

Basic collision models for 2-level system dynamics.

<img width="2816" height="1536" alt="open_quantum_systems" src="https://github.com/user-attachments/assets/52b7acbd-8372-496d-a506-630cdfe4c27b" />

<img width="2816" height="1536" alt="quantum_reservoir" src="https://github.com/user-attachments/assets/988032b8-95e5-4db9-84ef-c4526f4099a2" />

# Quantum Decoherence and Collision Models

This repository contains simulations of **Quantum Decoherence and Collision Models** that I developed as part of my Physics Engineering graduation project.

In this work, where we examine system-environment interactions, we model both memoryless (Markovian) and memory-environmental (Non-Markovian) quantum dynamics using the [QuTiP](https://qutip.org/) library in Python.

## 📂 Contents and Simulations

### 1. `Markovian_Analytical vs Collision Model.ipynb`

This file contains a simulation of **Markovian (Memoryless)** dynamics through a collision model.

- The environment (Ancilla) is included in the system in each collision in a "fresh" and "cold" ground state ($|0\rangle$). - An **Amplitude Damping** interaction simulating energy exchange has been established.
- The numerical coherence loss data obtained from the Collision Model is plotted comparatively with the analytical solution, the $\cos(g\tau)^n$ function.

### 2. `non_markov_strategies.ipynb`
This simulation examines a more complex structure where **Non-Markovian (Memory)** strategies are integrated into the system. - A **memory effect** is created in the system by establishing an interaction ($U_{AA}$) based on SWAP operators between successive ancillaries forming the environment.
- Memory power can be dynamically controlled with the $\theta$ parameter ($\theta = 0$ Markovian, $\theta = \pi/2$ Full Swap, $\theta = \pi/4$ Maximum Entanglement). - Time evolution was designed by taking the exponent from the Hamiltonian, ensuring that the matrix remains "Unitary" (probability-preserving).

<img width="839" height="521" alt="strat_2_full" src="https://github.com/user-attachments/assets/78b54029-8460-4c40-af78-d22ef519b36f" />

<img width="839" height="521" alt="strat_2_partial" src="https://github.com/user-attachments/assets/9992ca29-5a3f-45bb-b6c2-5b52f16458c4" />

<img width="839" height="521" alt="strat_1_theta" src="https://github.com/user-attachments/assets/c5b0358e-e26f-4d58-a9a8-c0a9b2b30625" />

**"Coherence Revival"** effects, where the information/energy lost by the system to the environment is returned to the system, have been successfully observed. 

## 🛠️ Technologies Used
- **Python 3.x**
- **QuTiP** (Quantum Toolbox in Python)
- **NumPy** (Physical parameters and matrix operations)
- **Matplotlib** (Visualization of superposition/coherence and trace graphs)
