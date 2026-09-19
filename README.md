# 🌉 Structural Damage & Concrete Crack Detection Model v2.0 (Enhanced)

<div align="center">

[![YOLOv8](https://img.shields.io/badge/YOLOv8-State%20of%20the%20Art-blue.svg?style=for-the-badge)](https://ultralytics.com)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.0+-EE4C2C.svg?style=for-the-badge&logo=pytorch)](https://pytorch.org)
[![Infrastructure AI](https://img.shields.io/badge/Civil%20AI-Structural%20Health-009688.svg?style=for-the-badge)](https://github.com)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](LICENSE)

**Advanced structural health monitoring and civil defect detection model with multi-tier severity grading for drone and robotic inspection.**

</div>

---

## 📌 Overview

**Concrete Cracks Detection v2.0** represents an upgraded computer vision pipeline engineered to automate the safety assessment of critical infrastructure (bridges, tunnels, highway overpasses, and high-rise foundations).

Upgraded with an expanded dataset, enhanced synthetic augmentations, and improved backbone feature extractors, v2.0 delivers superior precision in challenging lighting and shadowed environments.

---

## 🎯 Structural Damage Taxonomy & Severity

| Class ID | Class Name | Description | Severity Level |
| :---: | :--- | :--- | :---: |
| **0** | **Hairline Cracks** | Surface-level micro cracks (< 1mm width) | Low 🟢 |
| **1** | **Structural Fractures** | Deep penetration cracks affecting load distribution | High 🟠 |
| **2** | **Concrete Spalling** | Chipped and missing surface concrete | High 🟠 |
| **3** | **Exposed Rebar** | Corroded steel reinforcement visible | Critical 🔴 |

---

## ⚡ Key Enhancements in v2.0

- **🚀 Higher mAP@0.5**: Improved mean Average Precision across all fracture classes.
- **🎥 Video Stream Analysis**: Real-time batch inference on continuous inspection recordings (`Output_video.avi`).
- **🚁 Drone-Ready Architecture**: Calibrated to handle oblique camera angles and variable aerial zoom factors.

---

## 🛠️ Usage Instructions

1. **Clone and Install**:
   ```bash
   git clone https://github.com/<your-username>/concrete-cracks-detection2.0.git
   cd concrete-cracks-detection2.0
   pip install -r requirements.txt
   ```

2. **Run Video Inspection**:
   ```bash
   python detect.py --weights model/best.pt --source Output_video.avi
   ```

---

## 📄 License

Distributed under the **MIT License**. See [`LICENSE`](LICENSE) for details.
