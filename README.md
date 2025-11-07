# hPINN-Adver-Code
This program is a program for solving the optimal control problem of PDE constraints using the adversarial PINN method. If you refer to the program content, please cite our article.
Cao Y, So C C, Dai Y, et al. Adversarial physics-informed neural networks with hard constraints for optimal control of PDEs[J]. Journal of Computational Physics, 2025: 114307.

This repository presents an unsupervised neural network framework for solving PDE-constrained optimal control problems.
The approach leverages adversarial training to enhance the balance between physical constraints and optimization objectives.

🧠 Key Features

Adaptive hybrid PINN–GAN structure: Combines physics-informed learning with adversarial optimization to solve PDE-constrained control problems effectively.

Space–time dependent control variables: Supports control functions that vary across both spatial and temporal domains.

Dual-discriminator mechanism: The framework assigns separate discriminator networks to the physical residuals and the optimization objective, enabling them to adaptively update their relative weights during alternating adversarial training.

Classic Two-stage training strategy:

In the first stage, GAN hyperparameters and network architectures are determined through unsupervised training on representative PDE data. (Ref: Deqgan: Learning the loss function for pinns with generative adversarial networks)

In the second stage, the model jointly optimizes the state and control networks under the PDE constraint with dynamically balanced objectives.

All implementations are developed from scratch, following standard neural PDE-solving pipelines, and are designed for easy extension to new PDEs and control tasks.
