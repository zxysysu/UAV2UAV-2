# UAV2UAV-2

![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)
![Python 3.8+](https://img.shields.io/badge/python-3.8+-green.svg)
![Dataset Status](https://img.shields.io/badge/dataset-available-orange.svg)

## 项目简介
本项目对应论文 "Tracking A Fixed-Wing Unmanned Aerial Vehicle: An Experimental Evaluation"，核心贡献是构建了大规模、高多样性的固定翼无人机跟踪基准数据集（UAV2UAV-2），填补了现有 UAV2UAV 跟踪领域缺乏高质量训练数据与综合评估基准的空白。

## 核心贡献
1.  构建了 **UAV2UAV-2 基准数据集**：包含49段高清测试视频（27k+帧）和4.8k+训练图像，覆盖9类无人机跟踪核心挑战
2.  提供了 **24种主流跟踪算法的评估结果**：对比手工特征与深度学习特征跟踪器的性能差异
3.  开源了 **3种微调后的高性能跟踪器**：KYS-trained、Dimp18-trained、PrDimp-trained，提升了固定翼无人机跟踪的精度与成功率

## 数据集概况
| 数据类型 | 规格参数 |
|----------|----------|
| 测试视频 | 49段（30fps，3840×2160 分辨率） |
| 总帧数 | 27,000+（每帧含精准边界框标注） |
| 训练图像 | 4,800+张（1280×720 分辨率） |
| 覆盖挑战 | 低分辨率、运动模糊、光照变化、背景干扰等9类 |
| 标注格式 | JSON（边界框坐标 [x1, y1, x2, y2]） |

## 快速开始
### 1. 克隆仓库
```bash
git clone https://github.com/your-username/UAV2UAV-2.git
cd UAV2UAV-2
