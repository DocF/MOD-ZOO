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

## 📑 Table of Contents
<img align="right" width="47%" src="figures/publication.png" alt="MOD Publications over the past decade">

- [📢 News](#-news)
- [📝 Citation](#-citation)
- [📖 Abstract](#-abstract)
- [🖼️ Unified Framework & Taxonomy](#️-unified-framework--taxonomy)
- [🗂️ Datasets & Benchmarks](#️-datasets--benchmarks)
  - [Ground-based Datasets](#ground-based-datasets)
  - [Remote Sensing Datasets](#remote-sensing-datasets)
- [📚 Paper List (The MOD Zoo)](#-paper-list-the-mod-zoo)
  - [1. Feature Learning](#1-feature-learning-mitigating-representation-challenges)
  - [2. Fusion Scheme](#2-fusion-scheme)
  - [3. Detection Solutions](#3-detection-solutions-task-specific)

---

## 📢 News
* **[2026/04]** 🔥🔥The preprint will be available on arXiv soon!
* **[2026/04]** 🔥🔥Initial release of the **MOD-ZOO** repository, including taxonomy, datasets, and paper lists.

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
```

---

## 📖 Abstract

Multispectral Object Detection (MOD) has emerged as a critical methodology to overcome the limitations of visible-light imaging, particularly under adverse conditions such as low illumination and inclement weather. By integrating complementary information across diverse spectral bands, MOD ensures robust all-day and all-weather perception. 

To provide a systematic survey, a unified four-stage mathematical framework is established, which deconstructs MOD into **multispectral data input**, **feature learning**, **fusion schemes**, and **detection solutions**.

---

## 🖼️ Unified Framework & Taxonomy

Building upon the concepts introduced above, the following figures visualize the structural breakdown of our survey.

* **Figure 1** illustrates the detailed data flow of the unified mathematical framework, mapping the progression from raw multispectral inputs to final detection outputs.
* **Figure 2** expands this framework into a fine-grained hierarchical taxonomy. It categorizes recent state-of-the-art literature based on their specific strategies to overcome core cross-modal challenges.

*This taxonomy directly dictates the organization of the paper list in the following sections.*

<br>

<div align="center">
  <img src="figures/MOD.png" width="85%" alt="Unified Framework">
  <p><em>Figure 1. A unified four-stage framework and systematic taxonomy of MOD.</em></p>
</div>

<div align="center">
  <img src="figures/taxonomy.png" width="80%" alt="Taxonomy">
  <p><em>Figure 2. Hierarchical structural decomposition and taxonomy of the MOD landscape.</em></p>
</div>


## 🗂️ Datasets & Benchmarks

An overview of representative MOD datasets spanning ground-based and remote sensing scenarios.
<div align="center">
  <img src="figures/electromagnetic_spectrum2.png" width="80%" alt="Spectrum">
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
| AAAI'26 | IGIANet | Igianet: Illumination guided implicit alignment network for infrared-visible uav detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| TMM'25 | DeformCAT | Deformle cross-attention transformer for weakly aligned rgb-t pedestrin detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| TCSVT'25 | SeaDATE | Seadate: Remedy dual-attention transformer with semantic alignment via contrast learning for multimodal object detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| CVPR'24 | OAFA | Weakly misalignment-free adaptive feature alignment for uavs-based multimodal object detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| ECCV'24 | DAMSDet | Damsdet: Dynamic adaptive multispectral detection transformer with competitive query selection and adaptive feature fusion | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| ICIP'24 | L-CMAF | Revisiting misalignment in multispectral pedestrian detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| TIV'24 | YOLO-Adaptor | Yolo-adaptor: A fast adaptive one-stage detector for non-aligned visible-infrared object detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| MM'23 | AANet | Attentive alignment network for multispectral pedestrian detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| MM'23 | CALNet | Multispectral object detection via cross-modal conflict-aware learning | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| TITS'23 | MFPT | Multi-modal feature pyramid transformer for rgb-infrared object detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| ECCV'22 | TSFADet | Translation, scale and rotation: cross-modal alignment meets rgb-infrared vehicle detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| ICCV'19 | AR-CNN | Weakly aligned cross-modal learning for multispectral pedestrian detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |

#### Modality Imbalance

| Venue | Methods | Title | Modality | Source |
| :---: | :--- | :--- | :---: | :---: |
| TCSVT'25 | MSCoTDet | Mscotdet: Language-driven multi-modal fusion for improved multi-spectral pedestrian detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| TGRS'25 | DKDNet | Diffusion mechanism and knowledge distillation object detection in multimodal remote sensing imagery | <nobr>RGB-SAR</nobr> | [Paper](#)/[Code](#) |
| InfFus'25 | EMOD | Efficient multispectral object detection with attentive feature aggregation leveraging zero-shot implicit illumination guidance | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| ICCV'25 | M²D-LIF | Rethinking multi-modal object detection from the perspective of mono-modality feature learning | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| TITS'24 | MS-DETR | MS-DETR: multispectral pedestrian detection transformer with loosely coupled fusion and modality-balanced optimization | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| IROS'24 | DCSANet | Desanet: Dual cross-channel and spatial attention make RGB-T object detection better | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| CVPR'24 | CMM | Causal mode multiplexer: A novel framework for unbiased multispectral pedestrian detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| ECCV'22 | MBNet | Improving multispectral pedestrian detection by addressing modality imbalance problems | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |

#### Modality Redundancy

| Venue | Methods | Title | Modality | Source |
| :---: | :--- | :--- | :---: | :---: |
| NeuCom'24 | DHFNet | Dhfnet: Decoupled hierarchical fusion network for RGB-T dense prediction tasks | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| RS'22 | RISNet | Improving rgb-infrared object detection by reducing cross-modality redundancy | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| PR'22 | YOLOFusion | Cross-modality attentive feature fusion for object detection in multispectral remote sensing imagery | <nobr>RGB-NIR</nobr> | [Paper](#)/[Code](#) |

#### Modality Asymmetry

| Venue | Methods | Title | Modality | Source |
| :---: | :--- | :--- | :---: | :---: |
| MM'25 | UniRGB-IR | Unirgb-ir: A unified framework for visible-infrared semantic tasks via adapter tuning | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| ECCV'24 | ModTr | Modality translation for object detection adaptation without forgetting prior knowledge | <nobr>TIR</nobr> | [Paper](#)/[Code](#) |
| CVPR'24 | D3T | D3t: Distinctive dual-domain teacher zigzagging across rgb-thermal gap for domain-adaptive object detection | <nobr>TIR</nobr> | [Paper](#)/[Code](#) |
| MM'23 | TIRDet | Tirdet: Mono-modality thermal infrared object detection based on prior thermal-to-visible translation | <nobr>TIR</nobr> | [Paper](#)/[Code](#) |
| TCSVT'22 | DCRL-PDN | Deep cross-modal representation learning and distillation for illumination-invariant pedestrian detection | <nobr>RGB</nobr> | [Paper](#)/[Code](#) |
| AAAI'22 | VPD | Towards versatile pedestrian detector with multisensory-matching and multispectral recalling memory | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| ECCV'20 | TC-Det | Task-conditioned domain adaptation for pedestrian detection in thermal imagery | <nobr>TIR</nobr> | [Paper](#)/[Code](#) |
| CVPRW'19 | UMAD | Unsupervised domain adaptation for multispectral pedestrian detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| CVPR'17 | CMT-CNN | Learning cross-modal deep representations for robust pedestrian detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |

---

### 2. Fusion Scheme
Categorized by Fusion Stage Design and Fusion Function Construction.
<div align="center">
  <img src="figures/fusion-stage.png" width="100%" alt="Stage">
  <p><em>Figure 4. Fusion Stage Design.</em></p>
</div>
<div align="center">
  <img src="figures/fusion-func.png" width="80%" alt="Function">
  <p><em>Figure 5. Fusion Function Construction.</em></p>
</div>

| Venue | Methods | Title | Modality | Source |
| :---: | :--- | :--- | :---: | :---: |
| TIP'26 | <nobr>AFFNet</nobr> | Adaptive fine-grained fusion network for multimodal UAV object detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| InfFus'26 | <nobr>MSFF</nobr> | Multispectral state-space feature fusion: Bridging shared and cross-parametric interactions for object detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| InfFus'26 | <nobr>COMO</nobr> | COMO: cross-mamba interaction and offset-guided fusion for multimodal object detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| TII'25 | <nobr>RetinexDet</nobr> | Retinexdet: Enhancing multispectral object detection via retinex state space duality and wavelet-based frequency adaptive fusion | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| TGRS'25 | <nobr>MPFF</nobr> | Aerial image object detection based on rgb-infrared multibranch progressive fusion | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| TGRS'25 | <nobr>DHANet</nobr> | Dhanet: Dual-stream hierarchical interaction networks for multimodal drone object detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| TGRS'25 | <nobr>DMM</nobr> | DMM: disparity-guided multispectral mamba for oriented object detection in remote sensing | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| PR'25 | <nobr>MSTF</nobr> | Multispectral transformer fusion via exploiting similarity and complementarity for robust pedestrian detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| TMM'25 | <nobr>Fusion-Mamba</nobr> | Fusion-mamba for cross-modality object detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| MM'25 | <nobr>CSSFDet</nobr> | Contextually-guided state space fusion for misaligned multi-spectral object detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| MM'25 | <nobr>SemFusion</nobr> | Sam-guided semantic knowledge fusion for visible-infrared object detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| ICCV'25 | <nobr>WaveMamba</nobr> | Wavemamba: Wavelet-driven mamba fusion for rgb-infrared object detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| ICCV'25 | <nobr>M-SpecGene</nobr> | M-specgene: Generalized foundation model for rgbt multispectral vision | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| TNNLS'24| <nobr>LRAF-Net</nobr> | Lraf-net: Long-range attention fusion network for visible-infrared object detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| TNNLS'24| <nobr>TFDet</nobr> | Tfdet: Target-aware fusion for RGB-T pedestrian detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| ECCV'24 | <nobr>MMPedestron</nobr>| When pedestrian detection meets multi-modal learning: Generalist model and benchmark dataset | <nobr>Multi</nobr> | [Paper](#)/[Code](#) |
| NIPS'24 | <nobr>E2E-MFD</nobr> | E2e-mfd: Towards end-to-end synchronous multimodal fusion detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| TMM'23 | <nobr>CMPD</nobr> | Confidence-aware fusion using dempster-shafer theory for multispectral pedestrian detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| TCSVT'22| <nobr>UA-CMDet</nobr> | Drone-based rgb-infrared cross-modality vehicle detection via uncertainty-aware learning | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| InfFus'19 | <nobr>CIAN</nobr> | Cross-modality interactive attention network for multispectral pedestrian detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| PR'19 | <nobr>IAF R-CNN</nobr> | Illumination-aware faster r-cnn for robust multispectral pedestrian detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |

---

### 3. Detection Solutions (Task-Specific)
This section categorizes detection solutions based on specific application challenges: **Small Object Detection**, **Robust Perception Under Adverse Conditions**, and **Adversarial Attacks**.

#### Small Object Detection

| Venue | Methods | Title | Modality | Source |
| :---: | :--- | :--- | :---: | :---: |
| TIM'25 | <nobr>AMSDet</nobr> | Adaptive modality selection drone-based RGBT detector for tiny targets | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| TGRS'23 | <nobr>SuperYOLO</nobr> | Superyolo: Super resolution assisted object detection in multimodal remote sensing imagery | <nobr>RGB-NIR</nobr> | [Paper](#)/[Code](#) |
| ISPRS'23 | <nobr>QFDet</nobr> | Drone-based rgbt tiny person detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| BMVC'20 | <nobr>ASMPD</nobr> | Anchor-free small-scale multispectral pedestrian detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| ISPRS'19 | <nobr>HMFFN</nobr> | Box-level segmentation supervised deep neural networks for accurate and real-time multispectral pedestrian detection | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |


#### Robust Object Detection

| Venue | Methods | Title | Modality | Source |
| :---: | :--- | :--- | :---: | :---: |
| TCSVT'25 | <nobr>CFMW</nobr> | CFMW: cross-modality fusion mamba for robust object detection under adverse weather | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| PRL'25 | <nobr>RRD</nobr> | Learning a robust rgb-thermal detector for extreme modality imbalance | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| RAL'25 | <nobr>HA-MLPD</nobr> | Hybrid attention for robust RGB-T pedestrian detection in real-world conditions | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| MMUL'25 | <nobr>VL-ACFDet</nobr> | Vision-language-guided adaptive cross-modal fusion for multispectral object detection under adverse weather conditions | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| TGRS'24 | <nobr>LF-MDet</nobr> | Low-rank multimodal remote sensing object detection with frequency filtering experts | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| ECCV'20 | <nobr>ProbEn</nobr> | Multimodal object detection via probabilistic ensembling | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |


#### Adversarial Attack & Defense

| Venue | Methods | Title | Modality | Source |
| :---: | :--- | :--- | :---: | :---: |
| MM'25 | <nobr>CDUPatch</nobr> | Cdupatch: Color-driven universal adversarial patch attack for dual-modal visible-infrared detectors | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| TPAMI'24 | <nobr>UAPatch</nobr> | Unified adversarial patch for visible-infrared cross-modal attacks in the physical world | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| AAAI'23 | <nobr>MIC</nobr> | Multispectral invisible coating: Laminated visible-thermal physical attack against multispectral object detectors using transparent low-e films | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |
| ICASSP'23| <nobr>SRG-ASRP</nobr>| Similarity relation preserving cross-modal learning for multispectral pedestrian detection against adversarial attacks | <nobr>RGB-TIR</nobr> | [Paper](#)/[Code](#) |


*(Note: We welcome pull requests to update this list with the latest SOTA papers!)*


