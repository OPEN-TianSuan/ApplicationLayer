<div align="center">

Satellite application software organized by the OPEN-TianSuan community architecture, maintained by the **[OPEN-TianSuan](https://github.com/OPEN-TianSuan)** community.

[![Total views](https://raw.githubusercontent.com/OPEN-TianSuan/.github/main/traffic/ApplicationLayer.svg)](https://github.com/OPEN-TianSuan/.github/blob/main/traffic/ApplicationLayer.csv "Cumulative recorded repository views; updated hourly")
[![README](https://img.shields.io/badge/README-Chinese-blue?style=flat-square)](README.zh-CN.md)

**English** | [Chinese](README.zh-CN.md)

</div>

---

## 📂 Repository Layout

| Directory | Contents |
| --- | --- |
| [ImageClassificationSoftware](ImageClassificationSoftware/) | Visual perception applications. |
| [SituationalAwarenessSoftware](SituationalAwarenessSoftware/) | Attitude, change detection, ship detection and tracking applications. |
| [SatelliteNetworkingSoftware](SatelliteNetworkingSoftware/) | Cache, core network, compression and encoding applications. |
| [FoundationModelApplications](FoundationModelApplications/) | Reserved for foundation-model applications. |

## 📁 Directories

### ImageClassificationSoftware

- [ObjectDetection](ImageClassificationSoftware/ObjectDetection/) — YOLOv5-based general object detection.

### SituationalAwarenessSoftware

- [AttitudeDetermination](SituationalAwarenessSoftware/AttitudeDetermination/) — thermal-imagery attitude estimation.
- [ChangeDetectionAndEncoding](SituationalAwarenessSoftware/ChangeDetectionAndEncoding/) — cloud and illumination correction, change detection and selective encoding.
- [ShipDetection](SituationalAwarenessSoftware/ShipDetection/) — YOLOv5-based ship detection.
- [TrackingAlgorithm](SituationalAwarenessSoftware/TrackingAlgorithm/) — OpenCV optical-flow object tracking.

### SatelliteNetworkingSoftware

- [ClientCache](SatelliteNetworkingSoftware/ClientCache/) — client-side caching for satellite FaaS.
- [CoreNetwork](SatelliteNetworkingSoftware/CoreNetwork/) — 5G core network simulation with AMF, SMF and UPF.
- [DataCompression](SatelliteNetworkingSoftware/DataCompression/) — VAE-based image compression.
- [ImageEncoding](SatelliteNetworkingSoftware/ImageEncoding/) — JPEG image encoding.
- [MultiStageImageCompression](SatelliteNetworkingSoftware/MultiStageImageCompression/) — multi-stage image compression.

### FoundationModelApplications

Reserved for foundation-model applications.

> The ten application directories are the App1–App10 cases used in the ASE 2025 paper *SateLight: a satellite application update framework for satellite computing*.

## 🔗 Related Repositories

- [ComputeOperationsLayer](https://github.com/OPEN-TianSuan/ComputeOperationsLayer) — model training, inference and operations
- [InfrastructureLayer](https://github.com/OPEN-TianSuan/InfrastructureLayer) — platform management, runtime support and foundational software
- [EngineeringSupport](https://github.com/OPEN-TianSuan/EngineeringSupport) — development kits and evaluation platforms
- [SimulationPlatform](https://github.com/OPEN-TianSuan/SimulationPlatform) — satellite computing constellation simulation
- [SatelliteData](https://github.com/OPEN-TianSuan/SatelliteData) — remote sensing, orbital, telemetry and communication data
- [TechnicalLiterature](https://github.com/OPEN-TianSuan/TechnicalLiterature) — research papers, standards and documentation

## 🤝 Contributing

Researchers, developers, students and satellite enthusiasts are welcome. If you would like to contribute an application, open a pull request or start a discussion.

## 📄 License

Licenses and copyrights for each application remain with its original authors.
