<div align="center">

按 OPEN-TianSuan 社区内容架构组织的卫星应用软件，由 **[OPEN-TianSuan](https://github.com/OPEN-TianSuan)** 社区维护。

[![Total views](https://raw.githubusercontent.com/OPEN-TianSuan/.github/main/traffic/ApplicationLayer.svg)](https://github.com/OPEN-TianSuan/.github/blob/main/traffic/ApplicationLayer.csv "Cumulative recorded repository views; updated hourly")
[![README](https://img.shields.io/badge/README-English-blue?style=flat-square)](README.md)

[English](README.md) | **中文**

</div>

---

## 📂 仓库结构

| 目录 | 内容 |
| --- | --- |
| [ImageClassificationSoftware](ImageClassificationSoftware/) | 视觉感知类应用。 |
| [SituationalAwarenessSoftware](SituationalAwarenessSoftware/) | 姿态、变化检测、舰船检测与目标跟踪应用。 |
| [SatelliteNetworkingSoftware](SatelliteNetworkingSoftware/) | 缓存、核心网、压缩与编码应用。 |
| [FoundationModelApplications](FoundationModelApplications/) | 预留用于基础模型应用。 |

## 📁 目录说明

### ImageClassificationSoftware

- [ObjectDetection](ImageClassificationSoftware/ObjectDetection/) —— 基于 YOLOv5 的通用目标检测。

### SituationalAwarenessSoftware

- [AttitudeDetermination](SituationalAwarenessSoftware/AttitudeDetermination/) —— 基于热成像的姿态判定。
- [ChangeDetectionAndEncoding](SituationalAwarenessSoftware/ChangeDetectionAndEncoding/) —— 云与光照校正、变化检测与选择性编码。
- [ShipDetection](SituationalAwarenessSoftware/ShipDetection/) —— 基于 YOLOv5 的舰船检测。
- [TrackingAlgorithm](SituationalAwarenessSoftware/TrackingAlgorithm/) —— 基于 OpenCV 光流的目标跟踪。

### SatelliteNetworkingSoftware

- [ClientCache](SatelliteNetworkingSoftware/ClientCache/) —— 面向卫星 FaaS 的客户端缓存。
- [CoreNetwork](SatelliteNetworkingSoftware/CoreNetwork/) —— 基于 AMF、SMF、UPF 的 5G 核心网模拟。
- [DataCompression](SatelliteNetworkingSoftware/DataCompression/) —— 基于 VAE 的图像压缩。
- [ImageEncoding](SatelliteNetworkingSoftware/ImageEncoding/) —— JPEG 图像编码。
- [MultiStageImageCompression](SatelliteNetworkingSoftware/MultiStageImageCompression/) —— 多级图像压缩。

### FoundationModelApplications

预留用于基础模型应用。

> 十个应用目录即 ASE 2025 论文 *SateLight: a satellite application update framework for satellite computing* 中使用的 App1–App10。

## 🔗 相关仓库

- [ComputeOperationsLayer](https://github.com/OPEN-TianSuan/ComputeOperationsLayer) —— 模型训练、推理与运营
- [InfrastructureLayer](https://github.com/OPEN-TianSuan/InfrastructureLayer) —— 平台管理、运行支撑与基础软件
- [EngineeringSupport](https://github.com/OPEN-TianSuan/EngineeringSupport) —— 开发套件与评估平台
- [SimulationPlatform](https://github.com/OPEN-TianSuan/SimulationPlatform) —— 卫星计算星座仿真平台
- [SatelliteData](https://github.com/OPEN-TianSuan/SatelliteData) —— 遥感、轨道、遥测与通信数据
- [TechnicalLiterature](https://github.com/OPEN-TianSuan/TechnicalLiterature) —— 研究论文、标准与技术文档

## 🤝 参与贡献

欢迎研究人员、开发者、学生和卫星爱好者参与贡献。如需补充应用，欢迎提交 pull request 或发起讨论。

## 📄 许可

各应用的许可证与版权仍归其原作者所有。
