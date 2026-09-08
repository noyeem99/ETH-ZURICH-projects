Secure VFL: Cryptographic Aggregation & Differential Privacy

Introduction
This repository holds the implementation of a Secure Vertical Federated Learning (VFL) framework, built following the direction of Professor Kenny Paterson from ETH Zurich.The main goal of this project is to connect Applied Cryptography with Differential Privacy (DP). It shows how to connect data from multiple sources using cryptographic techniques and keeping it safe from privacy leaks using DP-SGD noise.

 1. Secure VFL Embedding Space Obfuscation

 File Name: secure_vfl_embedding_space_visualization.py

 Objective: Plot the embedding space to see how well the target boundaries are protected under Multi-Silo Distributed DP.

 Results: 

  Successfully hid 10 data clusters within the boundaries of X (-9 to 6) and Y (-7.5 to 10).

  Kept a clear separation between the red classes (Target: 1.0) and blue classes (Target: 0.0), proving the model works well even with differential privacy noise.

