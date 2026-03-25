# BabyEHANet
BabyEHANet: Lightweight Dual‑Residual Attention for Neonatal Behavior Monitoring
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

This repository contains the official implementation of **BabyEHANet**, a proof‑of‑concept edge‑deployable framework for vision‑based neonatal behavior monitoring. The system integrates a Dual‑Residual Enhanced Hybrid Attention (DR‑EHA) module into a MobileNetV3‑Small backbone to achieve robust classification of sleep/awake and crying/normal states under simulated NICU conditions (occlusions, variable lighting). The model is optimized for real‑time inference on a Raspberry Pi 5 using TensorFlow Lite.


## Features
- Novel DR‑EHA module with channel and spatial attention plus independent residual connections.
- Training on public infant face datasets (sleep/awake, crying/normal).
- Evaluation in a simulated NICU environment with controlled occlusions and lighting.
- Quantized TensorFlow Lite model with 8 ms inference latency on Raspberry Pi 5.
- End‑to‑edge pipeline (face detection → classification → alert via Firebase).
- Fully reproducible code with public datasets and simulation instructions.



## Setup

### Clone the repository
```bash
git clone https://github.com/yourusername/BabyEHANet.git
cd BabyEHANet
```
### Install dependencies
```bash
pip install -r requirements.txt
```
### Citation
If you use this code or find it helpful, please cite:

```
@article{mugisha2026babyehanet,
  title={BabyEHANet: A Lightweight Dual‑Residual Attention Network for Edge‑Based Neonatal Behavior Monitoring },
  author={Stanley Mugisha , Kisitu Rashid , Komakech Francis, Excellence Favor},
  journal={J },
  year={2026}
}
```

### License
This project is licensed under the MIT License – see the LICENSE file for details.

### Contact
For questions, open an issue or contact smugisha at sun dot ac dot ug.
