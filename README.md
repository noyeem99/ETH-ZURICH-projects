**Secure VFL: Cryptographic Aggregation & Differential Privacy**




Introduction
This repository holds the implementation of a Secure Vertical Federated Learning (VFL) framework, built following the direction of Professor Kenny Paterson from ETH Zurich.The main goal of this project is to connect Applied Cryptography with Differential Privacy (DP). It shows how to connect data from multiple sources using cryptographic techniques and keeping it safe from privacy leaks using DP-SGD noise.




 **1. Secure VFL Embedding Space Obfuscation**

 File Name: secure_vfl_embedding_space_visualization.py

 Objective: 
 
 Plot the embedding space to see how well the target boundaries are protected under Multi-Silo Distributed DP.

 Results: 

  Successfully hid 10 data clusters within the boundaries of X (-9 to 6) and Y (-7.5 to 10).

  Kept a clear separation between the red classes (Target: 1.0) and blue classes (Target: 0.0), proving the model works well even with differential privacy noise.

  

  

  **2. HE-DP Co-Design Framework Analysis**

 File Name: he_dp_codesign_framework.py

 Objective:
 
 Study the relationship between the Noise Multiplier (using Opacus Engine) and the Empirical Noise Variance (Utility Degradation Score).

  Results: 

  Successfully tracked how noise variance increases along with the noise multiplier from 0.5 to 3.0.

 Found that when the noise multiplier reaches 3.0, the noise variance peaks at around 9.5, showing exactly how much utility decreases as we push for stronger privacy.

 



 **3. GenAI Defense Auditing against Membership Inference Attacks**

 File Name: genai_defense_auditing.py

 Objective: 
 
 Test how well our Hybrid DP-Watermark defense drops the Attacker's Success Rate (MIA AUC Score) as the privacy noise increases.

 Results: 

   Proved that increasing the noise multiplier from 0.1 to 2.5 successfully forces the attacker's success rate down from over 90% to 50%.

   Hit the ideal random guessing limit (50% AUC) at around a 2.3 noise scale, meaning the model becomes perfectly protected against membership inference leaks.

