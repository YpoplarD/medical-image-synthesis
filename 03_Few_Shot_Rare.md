# Few-Shot & Rare Disease Synthesis

Methods designed for **extreme data imbalance**, **anatomy manipulation**, and **generating hard-to-acquire pathologies**.

* `AnoDDPM` [Wyatt et al., Proc. TMI 2022] **AnoDDPM: Anomaly Detection with Denoising Diffusion Probabilistic Models using Simplex Noise** [[PDF]](https://ieeexplore.ieee.org/document/9857019) [[CODE]](https://github.com/Julian-Wyatt/AnoDDPM)
  
  只学习健康数据，使用单纯形噪声
* `DeltaGAN` [Yan Hong et al., Proc. CVPR 2022] **DeltaGAN: Towards Diverse Few-shot Image Generation with Sample-Specific Delta** [[PDF]](https://arxiv.org/pdf/2009.08753) [[CODE]](https://github.com/bcmi/DeltaGAN-Few-Shot-Image-Generation)

  通用领域，从健康数据中学习变换（即不同健康个体之间的差别），再作用到小样本上以扩充数据量。（例：模型学习一个瘦的人、胖的人、正常身材的人的某个部位，之后将一张带病灶的样本扩充为这三种情况的三张/）
* `DAA-GAN` [Thermos et al., IEEE TMI 2021] **Controllable cardiac synthesis via disentangled anatomy arithmetic** [[PDF]](https://arxiv.org/abs/2107.01748v1) [[CODE]](https://github.com/vios-s/DAA-GAN)

  解剖和重构，将病变区域“移植”到健康数据上
* `DiffAugseg` [Jiaying Zhang et al., TMI 2024] **Data Augmentation in Class-Conditional Diffusion Model for Semi-Supervised Medical Image Segmentation** [[PDF]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10650822)
  
  提出一种基于类别属性（如疾病分期）引导的条件扩散模型，通过生成无标注的合成图像作为辅助数据，结合半监督学习框架提升了小样本数据集上的分割性能。
* `DiffAug` [Maham Nazir et al., ICCV 2025] **Diffusion-Based Data Augmentation for Medical Image Segmentation** [[PDF]](https://arxiv.org/abs/2508.17844)
  
  在健康图像上放上病灶，利用筛选机制选出合适的
* `Tiger Model` [Dai et al., Nature Communications 2025] **Improving AI models for rare thyroid cancer subtype by text‑guided diffusion models**[[PDF]](https://www.nature.com/articles/s41467-025-59478-8) [[CODE]](https://github.com/fangdai-dear/Tiger-Model)

  文本引导扩散模型：利用结构化临床文本和前景/背景双编码器，生成罕见甲状腺癌亚型的多样化超声图像
* `NeuroDiff-Aug` [Mallardi et al., Journal of Medical Systems 2025] **Diffusion Models for Neuroimaging Data Augmentation: Assessing Realism and Clinical Relevance** [[PDF]](https://link.springer.com/article/10.1007/s10916-025-02300-1)

  面向罕见神经影像场景，使用3D扩散模型生成脑MRI作为数据增强，通过统计指标与神经科专家主观评估双重验证合成图像的逼真度和临床可用性，核心贡献在评估。
* `GenFair-Med` [Ktena et al., Nature Medicine 2024] **Generative models improve fairness of medical classifiers** [[PDF]](https://pmc.ncbi.nlm.nih.gov/articles/PMC11031395/)

  利用可控扩散模型定向合成代表性不足的少数群体样本，对稀有数据标签扩展，模拟不同环境的数据分布偏移
* `SECONDGRAM` [Theodorou et al., Patterns 2025] **SECONDGRAM: Self-conditioned diffusion with gradient manipulation for longitudinal MRI imputation** [[PDF]](https://pmc.ncbi.nlm.nih.gov/articles/PMC11031395/)

  基于自条件扩散模型填补缺失时间点的影像，主要用于补全序列
* `Onto-CGAN` [Sun et al., npj Digital Medicine 2025] **Generating unseen diseases patient data using ontology enhanced generative adversarial networks** [[PDF]](https://www.nature.com/articles/s41746-024-01421-0) [[CODE]](https://github.com/sunchang0124/onto-cgan)
  
  利用疾病间的语义关联实现对未见疾病的特征合成
* `Lung-DDPM` [Jiang et al., IEEE TBME 2025] **Lung-DDPM: Semantic Layout-guided Diffusion Models for Thoracic CT Image Synthesis**[[PDF]](https://ieeexplore.ieee.org/document/11124548)[[CODE]](https://github.com/Manem-Lab/Lung-DDPM/)

  基于语义布局引导的3D扩散模型，通过输入包含解剖结构和结节位置的掩码生成高保真肺部CT图像
* `CXR‑LT` 2024 [Lin et al., Medical Image Analysis 2025] **CXR‑LT 2024: A MICCAI challenge on long‑tailed, multi‑label and zero‑shot chest X‑ray classification** [[PDF]](https://arxiv.org/abs/2506.07984)

  CXR‑LT 2024任务的基准介绍，对现有方法在长尾 + 零样本肺部疾病识别中的表现给出了系统分析，没有提出新方法
* `RaTrack` [T. Zhang et al., Electronics 2024] **Tracking the Rareness of Diseases: Improving Long‑Tail Chest X‑ray Detection with Diffusion Models** [[PDF]](https://www.mdpi.com/2079-9292/13/23/4693)

  专门针对稀有病种的 CXR 合成增强，先用扩散模型学习头部（常见病）分布，将尾类生成过程对齐到头类
* `Rare‑OCT Diffusion` [Iwanicka & Lu, MIUA 2025] **Diffusion with Adversarial Fine‑Tuning for Improving Rare Retinal Disease Diagnosis**[[PDF]](https://eprints.whiterose.ac.uk/id/eprint/228674/1/diffusion_camera_ready_Dominika%20Iwanicka%20and%20Ping%20Lu%20(1).pdf)

  DDPM + 注意力 + 类别感知 + 对抗微调生成少数类合成图像
* `Skin‑LDM` [M. Kim et al., PLOS ONE 2025] **Diffusion‑based skin disease data augmentation with fine‑tuned latent encoder–decoder** [[PDF]](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0331404)[[CODE]](https://github.com/raddshing/skin-disease-diffusion)

  基于stable diffusion，贡献一般，仅用clip改进编码器和解码器，有代码
* `AFLoc` [Yang et al., arXiv 2024] **A multi-modal vision-language model for generalizable annotation-free pathology localization** [[PDF]](https://arxiv.org/abs/2401.02044) [[CODE]](https://github.com/YH0517/AFLoc)

  解决无标注病理定位问题，多模态视觉‑语言语义对齐
* `GenSeg` [Zhang et al., Nat. Commun. 2025] **Generative AI enables medical image segmentation in ultra low-data regimes** [[PDF]](https://www.nature.com/articles/s41467-025-61754-6) [[CODE]](https://github.com/importZL/GenSeg)

  稀少样本医学分割，生成成对的图像‑掩码样本
