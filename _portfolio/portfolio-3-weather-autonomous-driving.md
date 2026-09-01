---
title: "How Bad Weather Affects the Safety of Autonomous Driving"
excerpt: "A research review of deep learning approaches to camera-based perception under adverse weather."
collection: portfolio
---

Autonomous vehicles rely on multiple sensors to interpret their surroundings, but there's ongoing debate about the minimal sensor array needed for safe, driverless operation while keeping manufacturing costs down. This research reviewed the literature on how computer vision performance degrades under adverse weather and noisy conditions, building the case for why multiple sensor modalities remain necessary.

The reviewed work largely relies on convolutional neural networks (CNNs) combined with recurrent neural networks (RNNs) to classify weather conditions and extract visual features from video frames. Three contemporary approaches YOLO, GRAMME, and ReViewNet were compared for how they reduce image noise and false edge detections across rain, snow, hail, and fog.

Results showed that snow and fog present the largest challenges for camera systems, with object detection accuracy dropping by over 20% across all methods tested, and average precision hovering around 50% well short of what's needed for safe autonomous operation. The review also highlighted that algorithm performance is highly dataset-dependent, and that the field needs standardized benchmarks to make fair comparisons between methods possible.

**Skills:** Research, technical writing, deep learning, computer vision, autonomous vehicles
