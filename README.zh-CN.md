[English](README.md) | **中文**

App1–App10 为 ASE 2025 论文中使用的应用。

下表列出十个应用目录。每个目录包含应用源码，以及运行所需的 Dockerfile 或构建文件。

| 应用 | 功能 | 实现 | 入口 |
| --- | --- | --- | --- |
| 姿态确定（Attitude Determination） | 从 16×12 的热成像图像估计航天器姿态：先将图像二值化为地球与天空，再据此判断卫星是否正确朝向，或绕相机轴发生了倾斜。 | Node.js；Dockerfile | `Attitude Determination/origin/index.js` |
| 变化检测与编码（Change Detection and Encoding） | 比较参考图像与当前拍摄图像，去除云层、对齐光照、检测变化区域，并仅对变化内容进行选择性编码。 | C++ 与 CMake；Dockerfile | `Change Detection and Encoding/origin/main.cpp` |
| 客户端缓存（Client Cache） | 面向卫星 FaaS 工作负载的客户端缓存，通过 gRPC 存储函数结果，使重复请求无需再次执行函数。 | Python、gRPC；模拟 FaaS 与 FRED 服务端；Dockerfile | `Client Cache/original/get_fn.py` 与 `Client Cache/original/put_fn.py` |
| 核心网（Core Network） | 模拟 5G 核心网的控制面行为，包括 AMF、SMF 与 UPF 网元。 | C；Dockerfile | `Core Network/origin/main.c` |
| 数据压缩（Data Compression） | 使用变分自编码器压缩卫星图像，提供高码率与低码率两套配置。 | PyTorch；VAE 模型与训练好的检查点；Dockerfile | `Data Compression/origin/compress.py` |
| 图像编码（Image Encoding） | 按可配置的质量参数将输入图像编码为 JPEG，为图像下行实验提供简单基线。 | Python 与 Pillow；Dockerfile | `Image Encoding/origin/encoding.py` |
| 多级图像压缩（Multi-Stage Image Compression） | 执行多级图像压缩流程，并输出样图的压缩结果。 | MATLAB；Dockerfile | `Multi-Stage Image Compression/origin/run_compression.m` |
| 目标检测（Object Detection） | 基于 YOLOv5 对图像进行目标检测，提供训练、验证、推理与模型导出脚本。 | YOLOv5 与 PyTorch；面向多种目标平台的 Dockerfile | `Object Detection/origin/detect.py` |
| 舰船检测（Ship Detection） | 使用 YOLOv5 模型与提供的预训练权重检测遥感图像中的舰船。 | YOLOv5 与 PyTorch；预训练权重 `best.pt`；Dockerfile | `Ship Detection/origin/detect.py` |
| 目标跟踪（Tracking Algorithm） | 使用 Shi–Tomasi 角点检测与金字塔 Lucas–Kanade 光流，在视频帧之间跟踪特征点。 | C++ 与 OpenCV；Dockerfile | `Tracking Algorithm/origin/main.cpp` |

Jinfeng Wen, Jianshu Zhao, Zixi Zhu, Xiaomin Zhang, Qi Liang, Ao Zhou, Shangguang Wang. SateLight: a satellite application update framework for satellite computing. Proceedings of the IEEE/ACM International Conference on Automated Software Engineering (ASE), 2025: 117-128.
