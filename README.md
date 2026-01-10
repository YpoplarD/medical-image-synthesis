# Awesome Medical Image Synthesis for Data Scarcity

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re) 
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)

This repository collects resources and papers on **Medical Image Synthesis**, with a special emphasis on tackling **Data Scarcity**, **Class Imbalance (Rare Diseases)**, and **Privacy Constraints**.

The organization of this repository is based on the **availability and nature of the training data** (Data-Centric Taxonomy).

## 🗂️ Contents (目录)

We classify the methods into the following categories based on data scenarios:

- **[1. Paired Image-to-Image Translation](./docs/1_paired_translation.md)**
  - *Scenario:* Rich datasets with pixel-to-pixel correspondence (e.g., MRI T1 $\leftrightarrow$ T2).
  
- **[2. Unpaired / Unsupervised Synthesis](./docs/2_unpaired_synthesis.md)**
  - *Scenario:* Two domains available but unaligned/unpaired (e.g., CT and MRI from different patient cohorts).

- **[3. Few-Shot & Rare Disease Synthesis](./docs/3_rare_disease_few_shot.md)** 🌟 **(Focus)**
  - *Scenario:* Extreme data scarcity, class imbalance, or longitudinal prediction (e.g., generating rare tumors, filling missing sessions).
  - *Keywords:* Disentanglement, Anomaly-to-Synthesis, Longitudinal Prediction.

- **[4. Text/Semantic-Guided Synthesis](./docs/4_controllable_synthesis.md)**
  - *Scenario:* Controllable generation using masks, biological parameters, or text prompts.
  - *Keywords:* Semantic Diffusion, ControlNet, Text-to-Image.

- **[5. Federated & Privacy-Preserving Generation](./docs/5_privacy_federated.md)**
  - *Scenario:* Distributed data that cannot be shared centrally due to privacy regulations.

## 📝 Citation

If you find this repository useful for your research, please consider starring ⭐ this repo.

```bibtex
@misc{awesome-medical-synthesis,
  author = {Yujie Yang},
  title = {Awesome Medical Image Synthesis for Data Scarcity},
  year = {2026},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{[https://github.com/yourusername/awesome-medical-image-synthesis](https://github.com/yourusername/awesome-medical-image-synthesis)}}
}
