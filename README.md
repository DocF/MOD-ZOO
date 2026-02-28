<div align="center">

# 🌟 Multispectral Object Detection: A Survey & MOD-ZOO

[![Paper](https://img.shields.io/badge/Paper-Arxiv-blue.svg)](#)
[![Awesome](https://awesome.re/badge.svg)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

**Qingyun Fang, Lingyun Gu, Guangwei Wen, Chunwu Liu, Xiaojun Liang, Zhaokui Wang, Rongyue Zheng, and Wen Gao**


---
**MOD-ZOO** is the official repository for the comprehensive survey paper **"Multispectral Object Detection: A Survey"**. It provides a unified framework, systematic taxonomy, and an open-source benchmark leaderboard for Multispectral Object Detection (MOD).

</div>

## 📢 News & Updates
* **[2026.02]** We release the initial version of **MOD-ZOO**, featuring comprehensive leaderboards and taxonomies covering 10+ datasets and 80+ state-of-the-art algorithms!
* **[2025.12]** Our survey paper is available on arXiv.

## 📖 Abstract
Multispectral Object Detection (MOD) has emerged as a critical methodology to overcome the limitations of visible-light imaging, particularly under adverse conditions such as low illumination and inclement weather. By integrating complementary information across diverse spectral bands (e.g., RGB, NIR, TIR, SAR), MOD ensures robust all-day and all-weather perception. 

This repository systematically deconstructs the MOD pipeline into a **unified four-stage mathematical framework**:
1. Multispectral Data Input
2. Feature Learning 
3. Fusion Schemes 
4. Detection Solutions.

---

## 🏗️ The Unified Four-Stage Framework

[cite_start]We establish a standardized foundation to inspire future research toward more robust and efficient multispectral vision systems[cite: 40]. 

<p align="center">
  <img src="assets/framework.png" alt="Four-Stage MOD Pipeline" width="800">
</p>
<p align="center">
  <em>Schematic illustration of the four-stage MOD pipeline. [cite_start]Modality-specific extractors encode inputs, aggregated via a cross-modal fusion mechanism, and decoded by the detection head[cite: 136].</em>
</p>

---

## 📚 Taxonomy of Representative Methods

We propose an extensive taxonomy of learning strategies designed to mitigate fundamental representation challenges. Below is a categorized overview of representative algorithms in the MOD landscape.

| Research Challenge | Representative Methods |
| :--- | :--- |
| **Small Object Detection** | [cite_start]HMFFN [7], ASMPD [21], QFDet [22], SuperYOLO [23], AMSDet [24], ProbEn [4] [cite: 150] |
| **Robust Object Detection** | [cite_start]LF-MDet [25], VL-ACFDet [26], HA-MLPD [27], RRD [28], CFMW [6] [cite: 150] |
| **Adversarial Attack** | [cite_start]SRG-ASRP [29], MIC [30] [cite: 150] |
| **Modality Misalignment** | [cite_start]AR-CNN [31], TSFADet [32], AANet [33], CALNet [34], MFPT [35], OAFA [36], DAMSDet [37], L-CMAF [38], YOLO-Adaptor [39], DeformCAT [40], SeaDATE [41] [cite: 150] |
| **Modality Imbalance** | [cite_start]MBNet [8], CMM [42], DCSANet [43], MS-DETR [44], EMOD [45], DKDNet [46] [cite: 150] |
| **Modality Redundancy** | [cite_start]MSCoTDet [47], YOLOFusion [48], RISNet [49], DHFNet [50] [cite: 150] |
| **Modality Adaption** | [cite_start]CMT-CNN [51], UMAD [52], TC-Det [53], VPD [54], DCRL-PDN [55], TIRDet [56], D3T [57], ModTr [58], M²D-LIF [5], UniRGB-IR [59] [cite: 150] |
| **Modality Fusion Schemes** | [cite_start]IAF R-CNN [60], CIAN [61], BAANet [62], UA-CMDet [63], CMPD [64], E2E-MFD [65], MMPedestron [66], TFDet [67], LRAF-Net [68], M-SpecGene [69], WaveMamba [70], SemFusion [71], CSSFDet [72], Fusion-Mamba [73], MSTF [74], DMM [75], DHANet [76], MPFF [77], MDFOaNet [78], RetinexDet [79], MSFF [80], COMO [81] [cite: 150] |

