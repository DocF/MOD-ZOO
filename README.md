# MOD-ZOO: Multispectral Object Detection - A Unified Framework and Systematic Survey

<div align="center">

[![Paper](https://img.shields.io/badge/Paper-arXiv-B31B1B.svg)](https://arxiv.org/)
[![Project Page](https://img.shields.io/badge/Project-MOD--ZOO-green.svg)](https://github.com/DocF/MOD-ZOO)
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

</div>

This is the official repository for the preprint paper **"Multispectral Object Detection: A Unified Framework and Systematic Survey"**. 

This repository (**MOD-ZOO**) provides a comprehensive, continuously updated collection of resources (papers, codes, datasets) for Multispectral Object Detection (MOD) across Ground-based and Remote Sensing scenarios.

---

## 📢 News
* **[2026/04]** The comprehensive survey paper has been submitted. The preprint will be available on arXiv soon!
* **[2026/04]** Initial release of the **MOD-ZOO** repository, including taxonomy, datasets, and paper lists.

---

## 📖 Abstract

Multispectral Object Detection (MOD) has emerged as a critical methodology to overcome the limitations of visible-light imaging, particularly under adverse conditions such as low illumination and inclement weather. By integrating complementary information across diverse spectral bands, MOD ensures robust all-day and all-weather perception. 

To provide a systematic survey, a unified four-stage mathematical framework is established, which deconstructs MOD into **multispectral data input**, **feature learning**, **fusion schemes**, and **detection solutions**.

---

## 🖼️ Unified Framework & Taxonomy

<div align="center">
  <img src="figures/MOD.png" width="85%" alt="Unified Framework">
  <p><em>Figure 1. A unified four-stage framework and systematic taxonomy of MOD.</em></p>
</div>

<div align="center">
  <img src="figures/taxonomy.png" width="80%" alt="Taxonomy">
  <p><em>Figure 2. Hierarchical structural decomposition and taxonomy of the MOD landscape.</em></p>
</div>

---

## 🗂️ Datasets & Benchmarks

An overview of representative MOD datasets spanning ground-based and remote sensing scenarios.
<div align="center">
  <img src="figures/electromagnetic_spectrum2.png" width="80%" alt="Taxonomy">
  <p><em>Figure 3. Electromagnetic spectrum mapping and visual comparisons.</em></p>
</div>

### Ground-based Datasets

### Ground-based Datasets

*(Legend: **Pairs** = Img Pairs, **Res.** = Resolution, **Plat.** = Platform, **Cls** = Class, **A/O** = Alignment / Occlusion)*

| Dataset | Venue | Modality | Pairs | Res. | Plat. | Cls | Den. | A/O | Link |
| :--- | :---: | :---: | :---: | :---: | :--- | :---: | :---: | :---: | :---: |
| KAIST | CVPR'15 | <nobr>RGB-TIR</nobr> | 95.3K | 640x480 | Driving | 1 | 0.62 | ✅/✅ | [Link](#) |
| CVC-14 | Sensors'16 | <nobr>RGB-TIR</nobr> | 8.5K | 640x512 | Driving | 1 | 0.80 | ❌/❌ | [Link](#) |
| FLIR-aligned | ICIP'20 | <nobr>RGB-TIR</nobr> | 5.1K | 640x512 | Driving | 3 | 7.92 | ✅/✅ | [Link](#) |
| LLVIP | ICCV'21 | <nobr>RGB-TIR</nobr> | 16.8K | 1080x720 | Surv. | 1 | 2.51 | ✅/❌ | [Link](#) |
| M³FD | CVPR'22 | <nobr>RGB-TIR</nobr> | 4.2K | 1024x768 | Multi. | 6 | 8.19 | ✅/❌ | [Link](#) |
| SMOD | TMM'25 | <nobr>RGB-TIR</nobr> | 8.6K | 640x512 | Driving | 4 | 3.62 | ✅/✅ | [Link](#) |
| MFAD | TCSVT'25 | <nobr>RGB-TIR</nobr> | 12.1K | 1280x960 | Driving | 6 | 7.13 | ✅/❌ | [Link](#) |



### Remote Sensing Datasets


*(Legend: **Pairs** = Img Pairs, **Res.** = Resolution, **Plat.** = Platform, **Cls** = Class, **A/O** = Alignment / Occlusion)*

| Dataset | Venue | Modality | Pairs | Res. | Plat. | Cls | Den. | A/O | Link |
| :--- | :---: | :---: | :---: | :---: | :--- | :---: | :---: | :---: | :---: |
| VEDAI | JVCI'16 | <nobr>R-NIR</nobr> | 1.2K | 1024x1024 | UAV | 9 | 2.93 | ✅/❌ | [Link](#) |
| DroneVehicle | TCSVT'21 | <nobr>R-TIR</nobr> | 28.4K | 840x712 | UAV | 1 | 16.7 | ❌/❌ | [Link](#) |
| DronePerson | ISPRS'23 | <nobr>R-TIR</nobr> | 6.1K | 640x512 | UAV | 1 | 11.6 | ✅/❌ | [Link](#) |
| DVTOD | TIV'24 | <nobr>R-TIR</nobr> | 2.1K | 1920x1080 | UAV | 3 | 2.82 | ❌/❌ | [Link](#) |
| OdinMJ | GRSM'24 | <nobr>R-TIR</nobr> | 23K | 640x512 | UAV | 1 | 1.98 | ✅/✅ | [Link](#) |
| RGBT-Tiny | TPAMI'25 | <nobr>R-TIR</nobr> | ~47.5K| 640x512 | UAV | 7 | 12.9 | ✅/❌ | [Link](#) |
| SpaceNet6-OTD| TGRS'22 | <nobr>R-SAR</nobr> | 820 | 900x900 | Sat. | 1 | 22.0 | ✅/❌ | [Link](#) |
| OGSOD-1.0 | TGRS'23 | <nobr>R-SAR</nobr> | 14.6K | 256x256 | Sat. | 3 | 2.62 | ✅/❌ | [Link](#) |
| OGSOD-2.0 | ICGIP'25 | <nobr>R-SAR</nobr> | 23.4K | 256x256 | Sat. | 4 | 3.24 | ✅/❌ | [Link](#) |


---

## 📚 Paper List (The MOD Zoo)

We categorize representative methods according to our proposed taxonomy.

### 1. Feature Learning (Mitigating Representation Challenges)
This section addresses fundamental representation challenges: spatial misalignment, modality imbalance, and information redundancy.

#### Modality Misalignment
| Year | Venue | Method | Title | Modality | Paper | Code |
| :--- | :---: | :--- | :--- | :---: | :---: | :---: |
| 2026 | AAAI | IGIANet | Illumination Guided Implicit Alignment Network for Infrared-Visible UAV Detection | RGB-TIR | [Paper](#) | [Code](#) |
| 2025 | TMM | DeformCAT | Deformable Cross-Attention Transformer for Weakly Aligned RGB-T Pedestrian Detection | RGB-TIR | [Paper](#) | [Code](#) |
| 2025 | TCSVT | SeaDATE | Remedy Dual-Attention Transformer with Semantic Alignment via Contrast Learning for Multimodal Object Detection | RGB-TIR | [Paper](#) | [Code](#) |
| 2024 | CVPR | OAFA | Weakly Misalignment-Free Adaptive Feature Alignment for UAVs-based Multimodal Object Detection | RGB-TIR | [Paper](#) | [Code](#) |
| 2024 | ECCV | DAMSDet | Dynamic Adaptive Multispectral Detection Transformer with Competitive Query Selection and Adaptive Feature Fusion | RGB-TIR | [Paper](#) | [Code](#) |
| 2023 | MM | AANet | Attentive Alignment Network for Multispectral Pedestrian Detection | RGB-TIR | [Paper](#) | [Code](#) |

#### Modality Imbalance
| Year | Venue | Method | Title | Modality | Paper | Code |
| :--- | :---: | :--- | :--- | :---: | :---: | :---: |
| 2025 | TGRS | BDFusion | Diffusion Mechanism and Knowledge Distillation Object Detection in Multimodal Remote Sensing Imagery | RGB-SAR | [Paper](#) | [Code](#) |
| 2025 | InfFus| EMOD | Efficient Multispectral Object Detection with Attentive Feature Aggregation Leveraging Zero-Shot Implicit Illumination Guidance | RGB-TIR | [Paper](#) | [Code](#) |
| 2025 | ICCV | $M^2D-LIF$ | Rethinking Multi-Modal Object Detection from the Perspective of Mono-Modality Feature Learning | RGB-TIR | [Paper](#) | [Code](#) |
| 2024 | CVPR | CMM | Causal Mode Multiplexer: A Novel Framework for Unbiased Multispectral Pedestrian Detection | RGB-TIR | [Paper](#) | [Code](#) |

#### Modality Redundancy & Asymmetry
| Year | Venue | Method | Title | Strategy | Paper | Code |
| :--- | :---: | :--- | :--- | :--- | :---: | :---: |
| 2025 | MM | UniRGB-IR | A Unified Framework for Visible-Infrared Semantic Tasks via Adapter Tuning | Adapter Tuning | [Paper](#) | [Code](#) |
| 2024 | ECCV | ModTr | Modality Translation for Object Detection Adaptation Without Forgetting Prior Knowledge | Modality Translation | [Paper](#) | [Code](#) |
| 2024 | NeuCom| DHFNet | Decoupled Hierarchical Fusion Network for RGB-T Dense Prediction Tasks | Redundancy Suppression | [Paper](#) | [Code](#) |

---

### 2. Fusion Scheme
Categorized by Fusion Stage Design and Fusion Function Construction.

#### Advanced Fusion Functions (Transformer & Mamba)
| Year | Venue | Method | Title | Backbone | Function | Paper | Code |
| :--- | :---: | :--- | :--- | :---: | :---: | :---: | :---: |
| 2026 | InfFus| MSFF | Multispectral State-Space Feature Fusion: Bridging Shared and Cross-Parametric Interactions for Object Detection | FCOS | Mamba | [Paper](#) | [Code](#) |
| 2025 | ICCV | M-SpecGene| Generalized Foundation Model for RGBT Multispectral Vision | ViTDet | Transformer | [Paper](#) | [Code](#) |
| 2025 | ICCV | WaveMamba | Wavelet-Driven Mamba Fusion for RGB-Infrared Object Detection | YOLOv8 | Mamba | [Paper](#) | [Code](#) |
| 2025 | TMM | Fusion-Mamba| Fusion-Mamba for Cross-Modality Object Detection | YOLOv8 | Mamba | [Paper](#) | [Code](#) |
| 2025 | PR | MSTF | Multispectral Transformer Fusion via Exploiting Similarity and Complementarity for Robust Pedestrian Detection | YOLOv5 | Transformer | [Paper](#) | [Code](#) |

---

### 3. Detection Solutions (Task-Specific)

| Category | Year | Venue | Method | Title | Key Idea | Paper | Code |
| :--- | :---: | :---: | :--- | :--- | :--- | :---: | :---: |
| **Robust** | 2025 | RAL | HA-MLPD | Hybrid Attention for Robust RGB-T Pedestrian Detection in Real-World Conditions | Hybrid attention prevents degradation under sensor blackouts | [Paper](#) | [Code](#) |
| **Robust** | 2025 | TCSVT | CFMW | CFMW: Cross-Modality Fusion Mamba for Robust Object Detection Under Adverse Weather | Mamba fusion integrates diffusion-based weather removal | [Paper](#) | [Code](#) |
| **Small Obj** | 2025 | TIM | AMSDet | Adaptive Modality Selection Drone-Based RGBT Detector for Tiny Targets | Adaptive selection filters redundancy for tiny object detection | [Paper](#) | [Code](#) |
| **Adversarial** | 2025 | MM | CDUPatch | Color-Driven Universal Adversarial Patch Attack for Dual-Modal Visible-Infrared Detectors | Color-thermal mapping for cross-modal adversarial textures | [Paper](#) | [Code](#) |

*(Note: We welcome pull requests to update this list with the latest SOTA papers!)*

---

## 📝 Citation

If you find this repository or our survey helpful for your research, please consider citing our paper:

```bibtex
@article{fang2024multispectral,
  title={Multispectral Object Detection: A Unified Framework and Systematic Survey},
  author={Fang, Qingyun and Gu, Lingyun and Wen, Guangwei and Liu, Chunwu and Liang, Xiaojun and Wang, Zhaokui and Zheng, Rongyue and Gao, Wen},
  journal={arXiv preprint},
  year={2026}
}
