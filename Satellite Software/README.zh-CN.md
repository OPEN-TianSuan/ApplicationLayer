<div align="center">

**Satellite Software** 是一个用于研究开源卫星相关软件生态的数据集与分析工具集。

[![README](https://img.shields.io/badge/README-English-blue?style=flat-square)](README.md)

[English](README.md) | **中文**

</div>

---

## 📂 收录内容

本目录介绍 **SatelliteSoftware** 研究仓库。源代码和数据集由独立的 [WenJinfeng/SatelliteSoftware 仓库](https://github.com/WenJinfeng/SatelliteSoftware)维护；本目录仅链接该工作，不将文件复制到 ApplicationLayer。

该仓库面向开源卫星相关软件的实证研究，强调数据采集、研究复现和后续复用的透明性。

## 🚀 内容概览

| 资源 | 说明 |
| --- | --- |
| `1-data_collection.py` | 采集与卫星相关的开源软件项目。 |
| `2-check_IsEnglish_readme.py` | 检查项目是否具有可访问的英文 README。 |
| `3-check_Iscontent.py` | 过滤仅包含 README、缺少实质内容的项目。 |
| `language_distribution_calculation.py` | 统计选定项目类别的编程语言分布。 |
| `All Satellite Projects for RQ1.xlsx` | 用于 RQ1、包含 22,286 个开源卫星相关项目的数据集。 |
| `Selected Projects for RQ2+RQ3.xlsx` | 用于 RQ2 和 RQ3、随机抽取的 646 个项目数据集。 |

## 📄 研究背景

该仓库配套论文 **Characterizing the Landscape of Open-Source Satellite Software**，论文已被 ASE 2026 接收。仓库公开了研究开源卫星软件规模、特征和编程语言分布时使用的数据采集脚本与数据集。

## 🚀 使用方法

克隆源码仓库以获取脚本、数据集和完整研究说明：

```bash
git clone https://github.com/WenJinfeng/SatelliteSoftware.git
cd SatelliteSoftware
```

数据采集流程、分析脚本、数据集定义和复现细节请参阅 [SatelliteSoftware 源码仓库](https://github.com/WenJinfeng/SatelliteSoftware)。

## 📌 来源与许可

源代码仓库：[https://github.com/WenJinfeng/SatelliteSoftware](https://github.com/WenJinfeng/SatelliteSoftware)。

本目录仅收录项目介绍并链接到外部源代码，不镜像脚本或数据集。当前许可证和版权归属信息请以源代码仓库为准。
