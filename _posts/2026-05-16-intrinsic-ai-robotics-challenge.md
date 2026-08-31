---
title: 'Intrinsic AI Robotics Challenge: Lessons in Dexterous Manipulation'
date: 2026-05-16
permalink: /posts/2026/05/intrinsic-ai-robotics-challenge/
tags:
  - Robotics
  - PhysicalAI
  - ImitationLearning
  - RoboticsChallenge
  - LeRobot
  - IntrinsicAI
---

My team and I recently participated in the Intrinsic AI Robotics Challenge, which focused on dexterous manipulation for electrical cable insertion, a complex but essential task in industrial automation.

I would like to thank my teammate Abelardo Garcia for collaborating with me on this project. It was quite challenging, we spent many evenings collecting data, debugging, and testing our policy designs. Both of us come from a robotics motion control background, and we were excited to apply our knowledge to this challenge. Through this process, we learned a great deal and had the opportunity to experiment with LeRobot from Hugging Face, which we plan to incorporate into our future projects.

Here are a few key takeaways regarding data collection:

1) The choice of simulation environment significantly impacts training quality
======
We used Gazebo, but in retrospect, training in Isaac Sim would have been advantageous due to its higher fidelity contact data, better visual resolution, and the ability to run parallel simulations which would have substantially increased our episode count. We should have invested in better hardware which would have enabled us to run Isaac Sim.

2) The quality and cleanliness of training data are crucial
======
Initially, we recorded overlapping data, which introduced conflicting trajectories into our dataset, rendering it unusable for training. The robot had no clear signal to learn from, so we had to discard that data and start fresh.

3) Diversity in data is essential
======
Our initial approach involved recording 100 episodes per position, one at a time, which proved to be inefficient for training. The model either failed to learn the insertion motion or overfitted, leading to stalls. When we introduced multiple positions, we encountered an imbalance in data distribution; the model fixated on one port position during testing and ignored others (regardless if we change the initial position). Moving forward, we would prioritize diverse episode collection across all positions, with more episodes to ensure better data generalization.

Thank you to Yadunund Vijay and the entire Intrinsic team for organizing a challenge that was both engaging and challenging. It provided students, industry professionals, and roboticists from various backgrounds a valuable opportunity to experiment, learn, and connect within the rapidly expanding robotics community.

Good luck to the remaining 30 teams.

#Robotics #PhysicalAI #ImitationLearning #RoboticsChallenge #LeRobot #IntrinsicAI
