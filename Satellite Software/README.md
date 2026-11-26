<div align="center">

**Satellite Software** is a dataset and analysis toolkit for studying the landscape of open-source satellite-related software.

[![README](https://img.shields.io/badge/README-Chinese-blue?style=flat-square)](README.zh-CN.md)

**English** | [Chinese](README.zh-CN.md)

</div>

---

## 📂 What Is Here

This directory introduces the **SatelliteSoftware** research repository. The source code and datasets are maintained in the standalone [WenJinfeng/SatelliteSoftware repository](https://github.com/WenJinfeng/SatelliteSoftware); this directory links to that work rather than copying its files into ApplicationLayer.

The repository supports empirical research on open-source satellite-related software, with an emphasis on transparent data collection, reproducibility, and reuse.

## 🚀 Contents

| Resource | Description |
| --- | --- |
| `1-data_collection.py` | Collects open-source software projects related to satellites. |
| `2-check_IsEnglish_readme.py` | Checks whether a project has an accessible English README. |
| `3-check_Iscontent.py` | Filters out projects that contain no substantial content beyond a README. |
| `language_distribution_calculation.py` | Calculates programming-language distributions for selected project categories. |
| `All Satellite Projects for RQ1.xlsx` | Dataset of 22,286 open-source satellite-related projects used for RQ1. |
| `Selected Projects for RQ2+RQ3.xlsx` | Curated dataset of 646 randomly selected projects used for RQ2 and RQ3. |

## 📄 Research Context

The repository accompanies the paper **Characterizing the Landscape of Open-Source Satellite Software**, accepted for publication at ASE 2026. It releases the collection scripts and datasets used to study the size, characteristics, and programming-language distribution of open-source satellite software.

## 🚀 Usage

Clone the source repository to access the scripts, datasets, and complete research documentation:

```bash
git clone https://github.com/WenJinfeng/SatelliteSoftware.git
cd SatelliteSoftware
```

See the [SatelliteSoftware repository](https://github.com/WenJinfeng/SatelliteSoftware) for the data collection workflow, analysis scripts, dataset definitions, and reproducibility details.

## 📌 Source and License

Source repository: [https://github.com/WenJinfeng/SatelliteSoftware](https://github.com/WenJinfeng/SatelliteSoftware).

This directory contains project information and links to the external source; it does not mirror the scripts or datasets. Check the source repository for current license and attribution information.
