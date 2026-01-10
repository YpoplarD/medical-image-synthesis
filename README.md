# Medical Image Synthesis

A curated list of resources focused on **Medical Image Synthesis**, emphasizing solutions for **Data Scarcity**, **Class Imbalance (Rare Diseases)**, and **Privacy Constraints**.

This repository organizes generative methods based on the **availability and nature of the training data**.

## Contents

The papers are categorized into the following sections based on the data scenario:

* **[1. Paired Image-to-Image Translation](01_Paired_Translation.md)**
    * *Scenario: Rich dataset with pixel-to-pixel correspondence (e.g., MRI T1 to T2).*
    * 针对拥有像素级对应配对数据的场景。

* **[2. Unpaired / Unsupervised Synthesis](02_Unpaired_Synthesis.md)**
    * *Scenario: Two domains available but unaligned (e.g., CT and MRI from different patients).*
    * 针对只有未对齐的双模态数据场景。

* **[3. Few-Shot & Rare Disease Synthesis](03_Few_Shot_Rare.md)**
    * *Scenario: Extreme data scarcity or class imbalance (e.g., generating rare tumors).*
    * 针对极度数据稀缺或类别不平衡（如罕见病）的场景。

* **[4. Text/Semantic-Guided Synthesis](04_Semantic_Guided.md)**
    * *Scenario: Controllable generation using masks, biological parameters, or text prompts.*
    * 利用掩码、生物参数或文本提示进行可控生成。

**[5. Distributed & Privacy-Constrained Synthesis](05_Distributed_Privacy.md)**
    * *Scenario: Data is abundant but fragmented across institutions (Data Silos) or restricted by privacy laws.*
    * 针对数据虽然存在，但分散在不同机构（数据孤岛）或受隐私法规限制无法集中的场景。
