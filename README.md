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

## 📢🔥 News
* **[2026/04]** 🔥🔥The comprehensive survey paper has been submitted. The preprint will be available on arXiv soon!
* **[2026/04]** 🔥🔥Initial release of the **MOD-ZOO** repository, including taxonomy, datasets, and paper lists.

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

*(Legend: **Pairs** = Img Pairs, **Res.** = Resolution, **Plat.** = Platform(Surv. = Surveillance, Multi. = Multiple), **Cls** = Class, **A/O** = Alignment / Occlusion)*
<div align="center">
  
| Dataset | Venue | Modality | Pairs | Res. | Plat. | Cls | Den. | A/O | Link |
| :--- | :---: | :---: | :---: | :---: | :--- | :---: | :---: | :---: | :---: |
| KAIST | CVPR'15 | <nobr>RGB-TIR</nobr> | 95.3K | 640x480 | Driving | 1 | 0.62 | ✅/✅ | [Link](#) |
| CVC-14 | Sensors'16 | <nobr>RGB-TIR</nobr> | 8.5K | 640x512 | Driving | 1 | 0.80 | ❌/❌ | [Link](#) |
| FLIR-aligned | ICIP'20 | <nobr>RGB-TIR</nobr> | 5.1K | 640x512 | Driving | 3 | 7.92 | ✅/✅ | [Link](#) |
| LLVIP | ICCV'21 | <nobr>RGB-TIR</nobr> | 16.8K | 1080x720 | Surv. | 1 | 2.51 | ✅/❌ | [Link](#) |
| M³FD | CVPR'22 | <nobr>RGB-TIR</nobr> | 4.2K | 1024x768 | Multi. | 6 | 8.19 | ✅/❌ | [Link](#) |
| SMOD | TMM'25 | <nobr>RGB-TIR</nobr> | 8.6K | 640x512 | Driving | 4 | 3.62 | ✅/✅ | [Link](#) |
| MFAD | TCSVT'25 | <nobr>RGB-TIR</nobr> | 12.1K | 1280x960 | Driving | 6 | 7.13 | ✅/❌ | [Link](#) |

</div>


### Remote Sensing Datasets


*(Legend: **Pairs** = Img Pairs, **Res.** = Resolution, **Plat.** = Platform, **Cls** = Class, **A/O** = Alignment / Occlusion)*
<div align="center">
  
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

</div>

---

## 📚 Paper List (The MOD Zoo)

We categorize representative methods according to our proposed taxonomy.

### 1. Feature Learning (Mitigating Representation Challenges)
This section addresses fundamental representation challenges: 
**Modality Misalignment**, **Modality Imbalance**, **Modality Redundancy**, and **Modality Asymmetry**.

#### Modality Misalignment

| Venue | Methods | Title | Modality | Source |
| :---: | :--- | :--- | :---: | :---: |
| AAAI'26 | IGIANet | Illumination Guided Implicit Alignment Network for Infrared-Visible UAV Detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| TMM'25 | DeformCAT | Deformable Cross-Attention Transformer for Weakly Aligned RGB-T Pedestrian Detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| TCSVT'25 | SeaDATE | Remedy Dual-Attention Transformer with Semantic Alignment via Contrast Learning for Multimodal Object Detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| CVPR'24 | OAFA | Weakly Misalignment-Free Adaptive Feature Alignment for UAVs-Based Multimodal Object Detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| ECCV'24 | DAMSDet | Dynamic Adaptive Multispectral Detection Transformer with Competitive Query Selection and Adaptive Feature Fusion | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| ICIP'24 | L-CMAF | Revisiting Misalignment in Multispectral Pedestrian Detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| TIV'24 | YOLO-Adaptor | A Fast Adaptive One-Stage Detector for Non-Aligned Visible-Infrared Object Detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| MM'23 | AANet | Attentive Alignment Network for Multispectral Pedestrian Detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| MM'23 | CALNet | Multispectral Object Detection via Cross-Modal Conflict-Aware Learning | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| TITS'23 | MFPT | Multi-Modal Feature Pyramid Transformer for RGB-Infrared Object Detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| ECCV'22 | TSFADet | Translation, Scale and Rotation: Cross-Modal Alignment Meets RGB-Infrared Vehicle Detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| ICCV'19 | AR-CNN | Weakly Aligned Cross-Modal Learning for Multispectral Pedestrian Detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |

#### Modality Imbalance
| Venue | Methods | Title | Modality | Source |
| :---: | :--- | :--- | :---: | :---: |
| TCSVT'25 | MSCoTDet | MSCoTDet: Language-Driven Multi-Modal Fusion for Improved Multi-Spectral Pedestrian Detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| TGRS'25 | DKDNet | Diffusion Mechanism and Knowledge Distillation Object Detection in Multimodal Remote Sensing Imagery | <nobr>RGB-SAR</nobr> | [Paper](#)/[Code](#) |
| InfFus'25 | EMOD | Efficient Multispectral Object Detection with Attentive Feature Aggregation Leveraging Zero-Shot Implicit Illumination Guidance | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| ICCV'25 | M²D-LIF | Rethinking Multi-Modal Object Detection from the Perspective of Mono-Modality Feature Learning | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| TITS'24 | MS-DETR | MS-DETR: Multispectral Pedestrian Detection Transformer with Loosely Coupled Fusion and Modality-Balanced Optimization | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| IROS'24 | DCSANet | DCSANet: Dual Cross-Channel and Spatial Attention Make RGB-T Object Detection Better | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| CVPR'24 | CMM | Causal Mode Multiplexer: A Novel Framework for Unbiased Multispectral Pedestrian Detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| ECCV'22 | MBNet | Improving Multispectral Pedestrian Detection by Addressing Modality Imbalance Problems | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |

</small>

#### Modality Redundancy & Asymmetry
| Venue | Methods | Title | Modality | Source |
| :---: | :--- | :--- | :---: | :---: |
| MM'25 | UniRGB-IR | A Unified Framework for Visible-Infrared Semantic Tasks via Adapter Tuning | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| ECCV'24 | ModTr | Modality Translation for Object Detection Adaptation Without Forgetting Prior Knowledge | <nobr>TIR</nobr> | [Paper](#)/[Code](#) |
| NeuCom'24| DHFNet | Decoupled Hierarchical Fusion Network for RGB-T Dense Prediction Tasks | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |

---

### 2. Fusion Scheme
Categorized by Fusion Stage Design and Fusion Function Construction.

#### Advanced Fusion Functions (Transformer & Mamba)
| Venue | Methods | Title | Modality | Source |
| :---: | :--- | :--- | :---: | :---: |
| InfFus'26| MSFF | Multispectral State-Space Feature Fusion: Bridging Shared and Cross-Parametric Interactions for Object Detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| ICCV'25 | M-SpecGene| Generalized Foundation Model for RGBT Multispectral Vision | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| ICCV'25 | WaveMamba | Wavelet-Driven Mamba Fusion for RGB-Infrared Object Detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| TMM'25 | Fusion-Mamba| Fusion-Mamba for Cross-Modality Object Detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| PR'25 | MSTF | Multispectral Transformer Fusion via Exploiting Similarity and Complementarity for Robust Pedestrian Detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |

---

### 3. Detection Solutions (Task-Specific)

| Venue | Methods | Title | Modality | Source |
| :---: | :--- | :--- | :---: | :---: |
| RAL'25 | HA-MLPD | Hybrid Attention for Robust RGB-T Pedestrian Detection in Real-World Conditions | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| TCSVT'25 | CFMW | CFMW: Cross-Modality Fusion Mamba for Robust Object Detection Under Adverse Weather | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| TIM'25 | AMSDet | Adaptive Modality Selection Drone-Based RGBT Detector for Tiny Targets | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| MM'25 | CDUPatch | Color-Driven Universal Adversarial Patch Attack for Dual-Modal Visible-Infrared Detectors | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |

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
