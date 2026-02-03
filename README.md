# UAV2UAV-2

![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)
![Python 3.8+](https://img.shields.io/badge/python-3.8+-green.svg)
![Dataset Status](https://img.shields.io/badge/dataset-available-orange.svg)

## Project Overview
This project corresponds to the paper **"Tracking A Fixed-Wing Unmanned Aerial Vehicle: An Experimental Evaluation"** by Yong Wang, Xiangyu Zhu, Zhiyang Sun, Robert Laganiere, and Lu Ding. The core contribution is the construction of the **UAV2UAV-2 dataset**—a large-scale, high-diversity benchmark for fixed-wing UAV tracking—filling the gap in the UAV-to-UAV (UAV2UAV) tracking domain, where high-quality training data and comprehensive evaluation benchmarks are lacking.

## Key Contributions
1. Developed the **UAV2UAV-2 benchmark dataset**: Includes 49 high-definition test videos (27k+ frames) and 4.8k+ training images, covering 9 core challenges in UAV tracking.
2. Provided evaluation results for **24 state-of-the-art tracking algorithms**: Compared performance differences between hand-crafted feature-based and deep learning-based trackers.
3. Open-sourced **3 fine-tuned high-performance trackers**: KYS-trained, Dimp18-trained, and PrDimp-trained, improving the accuracy and success rate of fixed-wing UAV tracking.

## Dataset Overview
| Data Type | Specifications |
|-----------|----------------|
| Test Videos | 49 sequences (30fps, 3840×2160 resolution) |
| Total Frames | 27,000+ (each frame with precise bounding box annotations) |
| Training Images | 4,800+ images (1280×720 resolution) |
| Covered Challenges | 9 types (low resolution, motion blur, illumination variation, background clutter, etc.) |
| Annotation Format | JSON (bounding box coordinates [x1, y1, x2, y2]) |

## Quick Start
### 1. Clone the Repository
```bash
git clone https://github.com/hapless19/UAV2UAV-2.git
cd UAV2UAV-2
