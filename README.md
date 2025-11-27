📘 Quantum Meta-Reinforcement Learning via Interference-Driven Policy Architectures

A physics-grounded exploration of generalization in RL through quantum interference

Author: Chetan Guduru

Status: Completed — Phase 1 

Paper: Quantum Meta-Reinforcement Learning via Interference-Driven Policy Architectures (QMRL)

⸻

🔥 Overview

This project introduces the first fixed-policy quantum meta-reinforcement learning framework where generalization emerges not through training, but through quantum interference.

We show that constructive interference encodes transferable action structure across tasks, enabling quantum agents to outperform classical heuristics in non-stationary and penalty-shaped environments.

The project consists of three phases:

	1.	Phase 1A — Environments
Three custom 5×5 grid-worlds with increasing complexity.

	2.	Phase 1B — Agent Evaluation
Six quantum circuits + classical baselines tested across 20 rollouts per task.

	3.	Phase 1C — Kernel Geometry & Theory
Quantum kernel matrices, PCA manifolds, interference sweeps, and a Hamiltonian-QFI analytical model.

The full paper includes analytical derivations, kernel geometry, noise/decoherence experiments, trajectory analysis, and a Q-learning baseline for comparison.

⸻

🧠 Key Idea

Instead of training a policy using gradients, we use constructive and destructive interference in quantum circuits to encode adaptable action distributions.

The central theoretical result:

Tr(FQ) = 4 Var(H)

This links Hamiltonian curvature to generalization ability, providing the first physics-grounded mechanism for inductive bias in quantum RL.

⸻

🌀 Quantum Circuits Implemented

Six architectures spanning interference-driven, entangled, and randomized models:

	1.	Quantum_Interference — H–CZ–RZ–H pattern
	
	2.	Quantum_HZH — H–Z–H interference sandwich
	
	3.	Quantum_Entangled — Bell-like initialization + mixed rotations
	
	4.	Quantum_Advanced — multi-axis entangled circuit
	
	5.	Quantum_Randomized — random rotations (non-interference baseline)
	
	6.	Quantum_CZDepth(k) — interference-depth sweep (k = 1–4)

Classical baselines include Greedy, Random, and Q-Learning.

⸻

📊 Core Results

1. Quantum agents generalize better on dynamic and penalty tasks.

Quantum_Interference and Quantum_HZH achieved:

	•	High stability on T2 (moving target)
	•	Near-perfect success on T3 (penalty field)
	•	Characteristic low-curvature behavior predicted by the Hamiltonian model

2. Quantum kernels form richer geometry than classical kernels.

Classical kernels collapse into diagonal noise.
Quantum kernels recover meaningful task clusters, smooth manifolds, and interference-aligned structure.

3. Constructive interference → adaptability.

Destructive interference → brittle specialization.
Matches both theory and empirical rollouts.

4. Noise & decoherence robustness.

Quantum kernels remain stable up to p ≈ 0.6, while classical kernels degrade immediately.

⸻

📐 Theoretical Contribution

🔹 The Hamiltonian–QFI Model

We derive a closed-form relationship linking:

	•	Hamiltonian variance
	•	Quantum Fisher information
	•	Generalization curvature

This provides a physical explanation for why interference helps agents adapt across related tasks.

🔹 Kernel Geometry Link

Interference strength predicts:

	•	task manifold structure
	•	cluster separability
	•	curvature peaks
	•	generalization zones (Δ ≈ 0)

⸻

🚀 Future Work

	•	Scale to larger or continuous-control environments
	•	Add learnable quantum meta-agents (hybrid VQC)
	•	Run circuits on real IBM hardware
	•	Expand classical baselines (PPO, A2C, RBF-meta-RL)

  I’m excited to take the interference-generalization idea from a promising 2-qubit prototype into the scale, theory, and hardware regime where it can become a real foundation for quantum machine learning.

⸻

📄 Citation

If you use this work, please cite:

C. Guduru, “Quantum Meta-Reinforcement Learning via Interference-Driven Policy Architectures,” 2025.

