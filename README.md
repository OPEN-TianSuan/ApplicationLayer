**English** | [Chinese](README.zh-CN.md)

App1 - App10 are used in the paper published in ASE 2025.

The ten application directories are listed below. Each directory contains the application source together with the Dockerfile or build files needed to run it.

| Application | Purpose | Implementation | Entry point |
| --- | --- | --- | --- |
| Attitude Determination | Estimates spacecraft attitude from a 16×12 thermal-camera image: the image is thresholded into Earth and sky, and the result indicates whether the satellite is correctly oriented or tilted about the camera axes. | Node.js; Dockerfile | `Attitude Determination/origin/index.js` |
| Change Detection and Encoding | Compares a reference image with a current capture, removes clouds, aligns illumination, detects changed regions, and selectively encodes only the changed content. | C++ with CMake; Dockerfile | `Change Detection and Encoding/origin/main.cpp` |
| Client Cache | Provides a client-side cache for satellite FaaS workloads, storing function results through gRPC so repeated requests can be served without re-executing the function. | Python, gRPC; mock FaaS and FRED servers; Dockerfile | `Client Cache/original/get_fn.py` and `Client Cache/original/put_fn.py` |
| Core Network | Simulates the control-plane behaviour of a 5G core network, including the AMF, SMF, and UPF network functions. | C; Dockerfile | `Core Network/origin/main.c` |
| Data Compression | Compresses satellite images with a variational autoencoder, with separate configurations for high-rate and low-rate compression. | PyTorch; VAE model and trained checkpoint; Dockerfile | `Data Compression/origin/compress.py` |
| Image Encoding | Encodes an input image as JPEG with a configurable quality level, providing a simple baseline for image downlink experiments. | Python and Pillow; Dockerfile | `Image Encoding/origin/encoding.py` |
| Multi-Stage Image Compression | Applies a multi-stage image-compression pipeline and reports the result for a sample input image. | MATLAB; Dockerfile | `Multi-Stage Image Compression/origin/run_compression.m` |
| Object Detection | Runs YOLOv5-based object detection on images, with scripts for training, validation, inference, and model export. | YOLOv5 and PyTorch; Dockerfiles for multiple targets | `Object Detection/origin/detect.py` |
| Ship Detection | Detects ships in remote-sensing images using a YOLOv5 model and the provided trained weights. | YOLOv5 and PyTorch; pre-trained `best.pt`; Dockerfile | `Ship Detection/origin/detect.py` |
| Tracking Algorithm | Tracks feature points across video frames using Shi–Tomasi corner detection and pyramidal Lucas–Kanade optical flow. | C++ and OpenCV; Dockerfile | `Tracking Algorithm/origin/main.cpp` |

## 🔗 Related Research Resource

The [Satellite Software](https://github.com/OPEN-TianSuan/ApplicationLayer/blob/main/Satellite%20Software/README.md) directory introduces the [WenJinfeng/SatelliteSoftware](https://github.com/WenJinfeng/SatelliteSoftware) dataset and analysis toolkit for studying open-source satellite-related software. The source scripts and datasets remain in the external repository.

Jinfeng Wen, Jianshu Zhao, Zixi Zhu, Xiaomin Zhang, Qi Liang, Ao Zhou, Shangguang Wang. SateLight: a satellite application update framework for satellite computing. Proceedings of the IEEE/ACM International Conference on Automated Software Engineering (ASE), 2025: 117-128.
