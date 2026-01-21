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

* `Few-shot DiffSeg` [Khosravi et al., Computers in Biology and Medicine 2023] Few-shot biomedical image segmentation using diffusion models: Beyond image generation (https://www.sciencedirect.com/science/article/abs/pii/S0169260723004984)

在中等规模生物医学图像上预训练 DDPM，将扩散过程中的特征作为辅助通道输入分割网络，在极少标注场景下显著提升分割性能。
* `NeuroDiff-Aug` [Mallardi et al., Journal of Medical Systems 2025] Diffusion Models for Neuroimaging Data Augmentation: Assessing Realism and Clinical Relevance (https://link.springer.com/article/10.1007/s10916-025-02300-1)

面向罕见神经影像场景，使用3D扩散模型生成脑MRI作为数据增强，通过统计指标与神经科专家主观评估双重验证合成图像的逼真度和临床可用性。
